# Example RPMs

1. List of [CentOS packages](https://centos.pkgs.org/7/centos-x86_64/).

## Content

1. [helm](#helm)
1. [my-sql-connector-java](#mysql-connector-java)
1. [kafka](#kafka)
1. [PostgreSQL](#postgresql)

## Helm

```console
# curl -X GET --output /tmp/test.rpm https://harbottle.gitlab.io/harbottle-main/7/x86_64/00871748-helm/helm-2.13.1-1.el7.harbottle.x86_64.rpm

# rpm -qlp /tmp/test.rpm
/usr/bin/helm
/usr/bin/rudder
/usr/bin/tiller
/usr/share/doc/helm-2.13.1
/usr/share/doc/helm-2.13.1/CONTRIBUTING.md
/usr/share/doc/helm-2.13.1/OWNERS
/usr/share/doc/helm-2.13.1/README.md
/usr/share/doc/helm-2.13.1/SECURITY_CONTACTS
/usr/share/doc/helm-2.13.1/code-of-conduct.md
/usr/share/licenses/helm-2.13.1
/usr/share/licenses/helm-2.13.1/LICENSE
```

## mysql-connector-java

```console
# curl -X GET --output /tmp/test.rpm http://repo.mysql.com/yum/mysql-connectors-community/el/7/i386//mysql-connector-java-8.0.15-1.el7.noarch.rpm

# rpm -qlp /tmp/test.rpm
/usr/share/doc/mysql-connector-java-8.0.15
/usr/share/doc/mysql-connector-java-8.0.15/CHANGES
/usr/share/doc/mysql-connector-java-8.0.15/INFO_BIN
/usr/share/doc/mysql-connector-java-8.0.15/INFO_SRC
/usr/share/doc/mysql-connector-java-8.0.15/LICENSE
/usr/share/doc/mysql-connector-java-8.0.15/README
/usr/share/java/mysql-connector-java-8.0.15.jar
```

## kafka

```console
# curl -X GET --output /tmp/test.rpm http://mirror.centos.org/centos/7/os/x86_64/Packages/librdkafka-0.11.4-1.el7.x86_64.rpm

# rpm -qlp /tmp/test.rpm
/usr/lib64/librdkafka++.so.1
/usr/lib64/librdkafka.so.1
/usr/lib64/pkgconfig/rdkafka++.pc
/usr/lib64/pkgconfig/rdkafka.pc
/usr/share/doc/librdkafka-0.11.4
/usr/share/doc/librdkafka-0.11.4/CONFIGURATION.md
/usr/share/doc/librdkafka-0.11.4/INTRODUCTION.md
/usr/share/doc/librdkafka-0.11.4/README.md
/usr/share/licenses/librdkafka-0.11.4
/usr/share/licenses/librdkafka-0.11.4/LICENSE
/usr/share/licenses/librdkafka-0.11.4/LICENSE.pycrc
/usr/share/licenses/librdkafka-0.11.4/LICENSE.snappy
```

## PostgreSQL

```console
# curl -X GET --output /tmp/test.rpm https://forensics.cert.org/centos/sip/7/x86_64//postgresql-server-9.3.4-1.el7.x86_64.rpm

# rpm -qlp /tmp/test.rpm
/etc/pam.d/postgresql
/usr/bin/initdb
/usr/bin/pg_basebackup
/usr/bin/pg_controldata
/usr/bin/pg_ctl
/usr/bin/pg_receivexlog
/usr/bin/pg_resetxlog
/usr/bin/postgres
/usr/bin/postgresql-check-db-dir
/usr/bin/postgresql-setup
/usr/bin/postmaster
/usr/lib/systemd/system/postgresql.service
/usr/lib/tmpfiles.d/postgresql.conf
/usr/lib64/pgsql/ascii_and_mic.so
/usr/lib64/pgsql/cyrillic_and_mic.so
/usr/lib64/pgsql/dict_snowball.so
/usr/lib64/pgsql/euc2004_sjis2004.so
/usr/lib64/pgsql/euc_cn_and_mic.so
/usr/lib64/pgsql/euc_jp_and_sjis.so
/usr/lib64/pgsql/euc_kr_and_mic.so
/usr/lib64/pgsql/euc_tw_and_big5.so
/usr/lib64/pgsql/latin2_and_win1250.so
/usr/lib64/pgsql/latin_and_mic.so
/usr/lib64/pgsql/libpqwalreceiver.so
/usr/lib64/pgsql/plpgsql.so
/usr/lib64/pgsql/utf8_and_ascii.so
/usr/lib64/pgsql/utf8_and_big5.so
/usr/lib64/pgsql/utf8_and_cyrillic.so
/usr/lib64/pgsql/utf8_and_euc2004.so
/usr/lib64/pgsql/utf8_and_euc_cn.so
/usr/lib64/pgsql/utf8_and_euc_jp.so
/usr/lib64/pgsql/utf8_and_euc_kr.so
/usr/lib64/pgsql/utf8_and_euc_tw.so
/usr/lib64/pgsql/utf8_and_gb18030.so
/usr/lib64/pgsql/utf8_and_gbk.so
/usr/lib64/pgsql/utf8_and_iso8859.so
/usr/lib64/pgsql/utf8_and_iso8859_1.so
/usr/lib64/pgsql/utf8_and_johab.so
/usr/lib64/pgsql/utf8_and_sjis.so
/usr/lib64/pgsql/utf8_and_sjis2004.so
/usr/lib64/pgsql/utf8_and_uhc.so
/usr/lib64/pgsql/utf8_and_win.so
/usr/libexec/initscripts/legacy-actions/postgresql
/usr/libexec/initscripts/legacy-actions/postgresql/initdb
/usr/libexec/initscripts/legacy-actions/postgresql/upgrade
/usr/share/locale/cs/LC_MESSAGES/initdb-9.3.mo
/usr/share/locale/cs/LC_MESSAGES/pg_basebackup-9.3.mo
/usr/share/locale/cs/LC_MESSAGES/pg_controldata-9.3.mo
/usr/share/locale/cs/LC_MESSAGES/pg_ctl-9.3.mo
/usr/share/locale/cs/LC_MESSAGES/pg_resetxlog-9.3.mo
/usr/share/locale/cs/LC_MESSAGES/plpgsql-9.3.mo
/usr/share/locale/de/LC_MESSAGES/initdb-9.3.mo
/usr/share/locale/de/LC_MESSAGES/pg_basebackup-9.3.mo
/usr/share/locale/de/LC_MESSAGES/pg_controldata-9.3.mo
/usr/share/locale/de/LC_MESSAGES/pg_ctl-9.3.mo
/usr/share/locale/de/LC_MESSAGES/pg_resetxlog-9.3.mo
/usr/share/locale/de/LC_MESSAGES/plpgsql-9.3.mo
/usr/share/locale/de/LC_MESSAGES/postgres-9.3.mo
/usr/share/locale/es/LC_MESSAGES/initdb-9.3.mo
/usr/share/locale/es/LC_MESSAGES/pg_basebackup-9.3.mo
/usr/share/locale/es/LC_MESSAGES/pg_controldata-9.3.mo
/usr/share/locale/es/LC_MESSAGES/pg_ctl-9.3.mo
/usr/share/locale/es/LC_MESSAGES/pg_resetxlog-9.3.mo
/usr/share/locale/es/LC_MESSAGES/plpgsql-9.3.mo
/usr/share/locale/es/LC_MESSAGES/postgres-9.3.mo
/usr/share/locale/fr/LC_MESSAGES/initdb-9.3.mo
/usr/share/locale/fr/LC_MESSAGES/pg_basebackup-9.3.mo
/usr/share/locale/fr/LC_MESSAGES/pg_controldata-9.3.mo
/usr/share/locale/fr/LC_MESSAGES/pg_ctl-9.3.mo
/usr/share/locale/fr/LC_MESSAGES/pg_resetxlog-9.3.mo
/usr/share/locale/fr/LC_MESSAGES/plpgsql-9.3.mo
/usr/share/locale/fr/LC_MESSAGES/postgres-9.3.mo
/usr/share/locale/it/LC_MESSAGES/initdb-9.3.mo
/usr/share/locale/it/LC_MESSAGES/pg_basebackup-9.3.mo
/usr/share/locale/it/LC_MESSAGES/pg_controldata-9.3.mo
/usr/share/locale/it/LC_MESSAGES/pg_ctl-9.3.mo
/usr/share/locale/it/LC_MESSAGES/pg_resetxlog-9.3.mo
/usr/share/locale/it/LC_MESSAGES/plpgsql-9.3.mo
/usr/share/locale/it/LC_MESSAGES/postgres-9.3.mo
/usr/share/locale/ja/LC_MESSAGES/initdb-9.3.mo
/usr/share/locale/ja/LC_MESSAGES/pg_basebackup-9.3.mo
/usr/share/locale/ja/LC_MESSAGES/pg_controldata-9.3.mo
/usr/share/locale/ja/LC_MESSAGES/pg_ctl-9.3.mo
/usr/share/locale/ja/LC_MESSAGES/pg_resetxlog-9.3.mo
/usr/share/locale/ja/LC_MESSAGES/plpgsql-9.3.mo
/usr/share/locale/ja/LC_MESSAGES/postgres-9.3.mo
/usr/share/locale/pl/LC_MESSAGES/initdb-9.3.mo
/usr/share/locale/pl/LC_MESSAGES/pg_basebackup-9.3.mo
/usr/share/locale/pl/LC_MESSAGES/pg_controldata-9.3.mo
/usr/share/locale/pl/LC_MESSAGES/pg_ctl-9.3.mo
/usr/share/locale/pl/LC_MESSAGES/pg_resetxlog-9.3.mo
/usr/share/locale/pl/LC_MESSAGES/plpgsql-9.3.mo
/usr/share/locale/pl/LC_MESSAGES/postgres-9.3.mo
/usr/share/locale/pt_BR/LC_MESSAGES/initdb-9.3.mo
/usr/share/locale/pt_BR/LC_MESSAGES/pg_basebackup-9.3.mo
/usr/share/locale/pt_BR/LC_MESSAGES/pg_controldata-9.3.mo
/usr/share/locale/pt_BR/LC_MESSAGES/pg_ctl-9.3.mo
/usr/share/locale/pt_BR/LC_MESSAGES/pg_resetxlog-9.3.mo
/usr/share/locale/pt_BR/LC_MESSAGES/plpgsql-9.3.mo
/usr/share/locale/pt_BR/LC_MESSAGES/postgres-9.3.mo
/usr/share/locale/ro/LC_MESSAGES/plpgsql-9.3.mo
/usr/share/locale/ru/LC_MESSAGES/initdb-9.3.mo
/usr/share/locale/ru/LC_MESSAGES/pg_basebackup-9.3.mo
/usr/share/locale/ru/LC_MESSAGES/pg_controldata-9.3.mo
/usr/share/locale/ru/LC_MESSAGES/pg_ctl-9.3.mo
/usr/share/locale/ru/LC_MESSAGES/pg_resetxlog-9.3.mo
/usr/share/locale/ru/LC_MESSAGES/plpgsql-9.3.mo
/usr/share/locale/ru/LC_MESSAGES/postgres-9.3.mo
/usr/share/locale/sv/LC_MESSAGES/pg_ctl-9.3.mo
/usr/share/locale/zh_CN/LC_MESSAGES/initdb-9.3.mo
/usr/share/locale/zh_CN/LC_MESSAGES/pg_basebackup-9.3.mo
/usr/share/locale/zh_CN/LC_MESSAGES/pg_controldata-9.3.mo
/usr/share/locale/zh_CN/LC_MESSAGES/pg_ctl-9.3.mo
/usr/share/locale/zh_CN/LC_MESSAGES/pg_resetxlog-9.3.mo
/usr/share/locale/zh_CN/LC_MESSAGES/plpgsql-9.3.mo
/usr/share/locale/zh_CN/LC_MESSAGES/postgres-9.3.mo
/usr/share/locale/zh_TW/LC_MESSAGES/pg_ctl-9.3.mo
/usr/share/locale/zh_TW/LC_MESSAGES/plpgsql-9.3.mo
/usr/share/locale/zh_TW/LC_MESSAGES/postgres-9.3.mo
/usr/share/man/man1/initdb.1.gz
/usr/share/man/man1/pg_basebackup.1.gz
/usr/share/man/man1/pg_controldata.1.gz
/usr/share/man/man1/pg_ctl.1.gz
/usr/share/man/man1/pg_receivexlog.1.gz
/usr/share/man/man1/pg_resetxlog.1.gz
/usr/share/man/man1/postgres.1.gz
/usr/share/man/man1/postgresql-setup.1.gz
/usr/share/man/man1/postmaster.1.gz
/usr/share/pgsql
/usr/share/pgsql/contrib
/usr/share/pgsql/conversion_create.sql
/usr/share/pgsql/extension
/usr/share/pgsql/extension/plpgsql--1.0.sql
/usr/share/pgsql/extension/plpgsql--unpackaged--1.0.sql
/usr/share/pgsql/extension/plpgsql.control
/usr/share/pgsql/information_schema.sql
/usr/share/pgsql/pg_hba.conf.sample
/usr/share/pgsql/pg_ident.conf.sample
/usr/share/pgsql/pg_service.conf.sample
/usr/share/pgsql/postgres.bki
/usr/share/pgsql/postgres.description
/usr/share/pgsql/postgres.shdescription
/usr/share/pgsql/postgresql.conf.sample
/usr/share/pgsql/psqlrc.sample
/usr/share/pgsql/recovery.conf.sample
/usr/share/pgsql/snowball_create.sql
/usr/share/pgsql/sql_features.txt
/usr/share/pgsql/system_views.sql
/usr/share/pgsql/timezonesets
/usr/share/pgsql/timezonesets/Africa.txt
/usr/share/pgsql/timezonesets/America.txt
/usr/share/pgsql/timezonesets/Antarctica.txt
/usr/share/pgsql/timezonesets/Asia.txt
/usr/share/pgsql/timezonesets/Atlantic.txt
/usr/share/pgsql/timezonesets/Australia
/usr/share/pgsql/timezonesets/Australia.txt
/usr/share/pgsql/timezonesets/Default
/usr/share/pgsql/timezonesets/Etc.txt
/usr/share/pgsql/timezonesets/Europe.txt
/usr/share/pgsql/timezonesets/India
/usr/share/pgsql/timezonesets/Indian.txt
/usr/share/pgsql/timezonesets/Pacific.txt
/usr/share/pgsql/tsearch_data
/usr/share/pgsql/tsearch_data/danish.stop
/usr/share/pgsql/tsearch_data/dutch.stop
/usr/share/pgsql/tsearch_data/english.stop
/usr/share/pgsql/tsearch_data/finnish.stop
/usr/share/pgsql/tsearch_data/french.stop
/usr/share/pgsql/tsearch_data/german.stop
/usr/share/pgsql/tsearch_data/hungarian.stop
/usr/share/pgsql/tsearch_data/hunspell_sample.affix
/usr/share/pgsql/tsearch_data/ispell_sample.affix
/usr/share/pgsql/tsearch_data/ispell_sample.dict
/usr/share/pgsql/tsearch_data/italian.stop
/usr/share/pgsql/tsearch_data/norwegian.stop
/usr/share/pgsql/tsearch_data/portuguese.stop
/usr/share/pgsql/tsearch_data/russian.stop
/usr/share/pgsql/tsearch_data/spanish.stop
/usr/share/pgsql/tsearch_data/swedish.stop
/usr/share/pgsql/tsearch_data/synonym_sample.syn
/usr/share/pgsql/tsearch_data/thesaurus_sample.ths
/usr/share/pgsql/tsearch_data/turkish.stop
/usr/share/pgsql/tsearch_data/unaccent.rules
/usr/share/pgsql/tsearch_data/xsyn_sample.rules
/var/lib/pgsql
/var/lib/pgsql/.bash_profile
/var/lib/pgsql/backups
/var/lib/pgsql/data
/var/run/postgresql
```
