# senzing-rpm

## Overview

## Example RPMs

1. [Example RPMs](docs/example-rpms)

## Guiding principles

The following "guiding principles" apply to `/opt` AddOns:

1. Use of `/opt`, `/var/opt`, and `/etc/opt`:
    > Under no circumstances are other package files to exist outside the /opt, /var/opt, and /etc/opt hierarchies except for those package files that must reside in specific locations within the filesystem tree in order to function properly. For example, device lock files in /var/lock and devices in /dev. Distributions may install software in /opt, but must not modify or delete software installed by the local system administrator without the assent of the local system administrator.
    > -- *[Linux Filesystem Hierarchy: 1.13 /opt](https://www.tldp.org/LDP/Linux-Filesystem-Hierarchy/html/opt.html)*
1. Use of `/usr/local`:
    > These days, '/usr/local' is widely regarded as a good place in which to keep self-compiled or third-party programs. The /usr/local hierarchy is for use by the system administrator when installing software locally. It needs to be safe from being overwritten when the system software is updated. It may be used for programs and data that are shareable amongst a group of hosts, but not found in /usr. Locally installed software must be placed within /usr/local rather than /usr unless it is being installed to replace or upgrade software in /usr.
    > -- *[Linux Filesystem Hierarchy:  1.17 /usr](https://www.tldp.org/LDP/Linux-Filesystem-Hierarchy/html/usr.html)*
1. Use of `/var/local`:
    > Variable data for local programs (i.e., programs that have been installed by the system administrator) that are installed in /usr/local (as opposed to a remotely mounted '/var' partition). Note that even locally installed programs should use the other /var directories if they are appropriate, e.g., /var/lock.
    > -- *[Linux Filesystem Hierarchy:  1.18 /var](https://www.tldp.org/LDP/Linux-Filesystem-Hierarchy/html/var.html)*

## Proposals

1. [Proposal 1](docs/proposal-1)

## Use in Docker

1. To share static files (i.e. can be mounted as Read-Only).
   **Note:** This saves 3GB per running container.

    ```console
    sudo docker run \
    --volume ${MY_STATIC_DIR}:/opt/senzing \
    senzing/xxxxx
    ```

1. To share configuration:

    ```console
    sudo docker run \
    --volume ${MY_CONFIG_DIR}:/etc/opt/senzing \
    senzing/xxxxx
    ```

1. To share files that can be changed by programs running in the container
   or state that needs to be saved across docker deployments:

    ```console
    sudo docker run \
    --volume ${MY_VAR_DIR}:/var/opt/lib/senzing \
    senzing/xxxxx
    ```

1. All together:

    ```console
    sudo docker run \
    --volume ${MY_STATIC_DIR}:/opt/senzing \
    --volume ${MY_CONFIG_DIR}:/etc/opt/senzing \
    --volume ${MY_VAR_DIR}:/var/opt/lib/senzing \
    senzing/xxxxx
    ```

1. This allows containers to share static code, but different configuration (i.e. different database instances)

## Questions

1. Are we product (`/opt`) or part of system?
1. Can we use "requires/dependencies" to use transitive package management?

## References

1. [Wikipedia: Filesystem Hierarchy Standard](https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard)
1. [Debian: FilesystemHierarchyStandard](https://wiki.debian.org/FilesystemHierarchyStandard)
1. [RedHat: Chapter 2. File System Structure and Maintenance](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/6/html/storage_administration_guide/ch-filesystem)
1. [Filesystem Hierarchy Standard, LSB Workgroup, The Linux Foundation](https://refspecs.linuxfoundation.org/FHS_3.0/fhs-3.0.pdf)
1. [The Linux Documentation Project: Chapter 1. Linux Filesystem Hierarchy](https://www.tldp.org/LDP/Linux-Filesystem-Hierarchy/html/c23.html)
1. [The Linux Directory Structure, Explained](https://www.howtogeek.com/117435/htg-explains-the-linux-directory-structure-explained/)
1. [RPM Dependencies](https://rpm.org/user_doc/dependencies.html)
