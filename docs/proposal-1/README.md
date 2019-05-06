# Proposal 1

## Overview

Directories used:

1. **Configuration**
    1. /etc/opt/senzing
1. **Static files**    
    1. /opt/senzing
1. **Varying files**    
    1. /var/opt/lib/senzing
    1. /var/opt/lib/senzing/sqlite

## Details

In "New location", a dash "`-`" means no change from "Old location". File list captured 5/6 from senzing-1.9.19126-1.x86_64.rpm


| Old location | New location | Notes |
|--------------|--------------|--------------|
| /opt/senzing/g2/LICENSE |-|
| /opt/senzing/g2/NOTICES |-|
| /opt/senzing/g2/README.1ST |-|
| /opt/senzing/g2/bin/saltadm |-|
| /opt/senzing/g2/bin/ssadm |-|
| /opt/senzing/g2/data/CFG_STB_ASSIGN.csv |-|
| /opt/senzing/g2/data/CFG_STB_MASTER.csv |-|
| /opt/senzing/g2/data/G2C.db |???| This also exists in g2/sqldb |
| /opt/senzing/g2/data/G2Module.ini | /etc/opt/senzing/G2Module.ini | We have two G2Module.ini currently, one in data and one in python. this would consoldate into on in etc |
| /opt/senzing/g2/data/G2Project.ini | /etc/opt/senzing/G2Project.ini | We have two G2Project.ini currently, one in data and one in python. this would consoldate into on in etc |
| /opt/senzing/g2/data/addressParserMetaData.xml |-|
| /opt/senzing/g2/data/angloOnRegRule.ibm |-|
| /opt/senzing/g2/data/angloRegRule.ibm |-|
| /opt/senzing/g2/data/anyTransRule.ibm |-|
| /opt/senzing/g2/data/arabicTransRule.ibm |-|
| /opt/senzing/g2/data/cfgVariant.json | /etc/opt/senzing/cfgVariant.json|
| /opt/senzing/g2/data/chineseNativeOnRegRule.ibm |-|
| /opt/senzing/g2/data/chineseOnRegRule.ibm |-|
| /opt/senzing/g2/data/chineseOnTransRule.ibm |-|
| /opt/senzing/g2/data/chineseRegRule.ibm |-|
| /opt/senzing/g2/data/chineseTransRule.ibm |-|
| /opt/senzing/g2/data/cnv.ibm |-|
| /opt/senzing/g2/data/conv.ibm |-|
| /opt/senzing/g2/data/ctaq.ibm |-|
| /opt/senzing/g2/data/customGn.txt | /etc/opt/senzing/customGn.txt |
| /opt/senzing/g2/data/customOn.txt | /etc/opt/senzing/customOn.txt |
| /opt/senzing/g2/data/customSn.txt | /etc/opt/senzing/customSn.txt |
| /opt/senzing/g2/data/cyrillicOnTransRule.ibm |-|
| /opt/senzing/g2/data/cyrillicTransRule.ibm |-|
| /opt/senzing/g2/data/defaultGNRCP.config |???|
| /opt/senzing/g2/data/errules_normal.umf |-|
| /opt/senzing/g2/data/errules_optimistic.umf |-|
| /opt/senzing/g2/data/errules_pessimistic.umf |-|
| /opt/senzing/g2/data/farsiRegRule.ibm |-|
| /opt/senzing/g2/data/flemish_germanRegRule.ibm |-|
| /opt/senzing/g2/data/frenchRegRule.ibm |-|
| /opt/senzing/g2/data/g2BuildVersion.json |-|
| /opt/senzing/g2/data/g2SifterRules.ibm |-|
| /opt/senzing/g2/data/g2config.json |/etc/opt/senzing/g2config.json| We have two g2config.json currently, one in data and one in python. this would consoldate into on in etc |
| /opt/senzing/g2/data/g2core-schema-db2-create.sql |-|
| /opt/senzing/g2/data/g2core-schema-db2-upgrade-1.1-to-1.2.sql |-|
| /opt/senzing/g2/data/g2core-schema-db2-upgrade-1.2-to-1.3.sql |-|
| /opt/senzing/g2/data/g2core-schema-db2-upgrade-1.3-to-1.4.sql |-|
| /opt/senzing/g2/data/g2core-schema-mysql-create.sql |-|
| /opt/senzing/g2/data/g2core-schema-mysql-upgrade-1.1-to-1.2.sql |-|
| /opt/senzing/g2/data/g2core-schema-mysql-upgrade-1.2-to-1.3.sql |-|
| /opt/senzing/g2/data/g2core-schema-mysql-upgrade-1.3-to-1.4.sql |-|
| /opt/senzing/g2/data/g2core-schema-postgresql-create.sql |-|
| /opt/senzing/g2/data/g2core-schema-sqlite-create.sql |-|
| /opt/senzing/g2/data/g2core-schema-sqlite-upgrade-1.1-to-1.2.sql |-|
| /opt/senzing/g2/data/g2core-schema-sqlite-upgrade-1.2-to-1.3.sql |-|
| /opt/senzing/g2/data/g2core-schema-sqlite-upgrade-1.3-to-1.4.sql |-|
| /opt/senzing/g2/data/genericOnRegRule.ibm |-|
| /opt/senzing/g2/data/genericRegRule.ibm |-|
| /opt/senzing/g2/data/germanRegRule.ibm |-|
| /opt/senzing/g2/data/gnv.ibm |-|
| /opt/senzing/g2/data/greekTransRule.ibm |-|
| /opt/senzing/g2/data/hindiOnTransRule.ibm |-|
| /opt/senzing/g2/data/hindiTransRule.ibm |-|
| /opt/senzing/g2/data/hispanicOnRegRule.ibm |-|
| /opt/senzing/g2/data/hispanicRegRule.ibm |-|
| /opt/senzing/g2/data/indianRegRule.ibm |-|
| /opt/senzing/g2/data/indoRegRule.ibm |-|
| /opt/senzing/g2/data/japaneseNativeOnRegRule.ibm |-|
| /opt/senzing/g2/data/japaneseOnTransRule.ibm |-|
| /opt/senzing/g2/data/japaneseRegRule.ibm |-|
| /opt/senzing/g2/data/japaneseTransRule.ibm |-|
| /opt/senzing/g2/data/koreanOnRegRule.ibm |-|
| /opt/senzing/g2/data/koreanOnTransRule.ibm |-|
| /opt/senzing/g2/data/koreanRegRule.ibm |-|
| /opt/senzing/g2/data/koreanTransRule.ibm |-|
| /opt/senzing/g2/data/libpostal/address_expansions/address_dictionary.dat |-|
| /opt/senzing/g2/data/libpostal/address_parser/address_parser_crf.dat |-|
| /opt/senzing/g2/data/libpostal/address_parser/address_parser_phrases.dat |-|
| /opt/senzing/g2/data/libpostal/address_parser/address_parser_postal_codes.dat |-|
| /opt/senzing/g2/data/libpostal/address_parser/address_parser_vocab.trie |-|
| /opt/senzing/g2/data/libpostal/data_version |-|
| /opt/senzing/g2/data/libpostal/language_classifier/language_classifier.dat |-|
| /opt/senzing/g2/data/libpostal/last_updated |-|
| /opt/senzing/g2/data/libpostal/last_updated_language_classifier |-|
| /opt/senzing/g2/data/libpostal/last_updated_parser |-|
| /opt/senzing/g2/data/libpostal/numex/numex.dat |-|
| /opt/senzing/g2/data/libpostal/transliteration/transliteration.dat |-|
| /opt/senzing/g2/data/mapping-templates/default-templates.tpl |-|
| /opt/senzing/g2/data/onv.ibm |-|
| /opt/senzing/g2/data/polishOnRegRule.ibm |-|
| /opt/senzing/g2/data/polishRegRule.ibm |-|
| /opt/senzing/g2/data/portugueseOnRegRule.ibm |-|
| /opt/senzing/g2/data/portugueseRegRule.ibm |-|
| /opt/senzing/g2/data/russianOnRegRule.ibm |-|
| /opt/senzing/g2/data/russianRegRule.ibm |-|
| /opt/senzing/g2/data/snv.ibm |-|
| /opt/senzing/g2/data/stb.config |???? |
| /opt/senzing/g2/data/swasianRegRule.ibm |-|
| /opt/senzing/g2/data/taq.ibm |-|
| /opt/senzing/g2/data/terms.ibm |-|
| /opt/senzing/g2/data/thaiRegRule.ibm |-|
| /opt/senzing/g2/lib/debian/libcrypto.so.10 |-|
| /opt/senzing/g2/lib/debian/libssl.so.10 |-|
| /opt/senzing/g2/lib/g2.jar |-|
| /opt/senzing/g2/lib/libDefaultRelationship.so |-|
| /opt/senzing/g2/lib/libG2.so |-|
| /opt/senzing/g2/lib/libG2Hasher.so |-|
| /opt/senzing/g2/lib/libG2SSAdm.so |-|
| /opt/senzing/g2/lib/libNameDataObject.so |-|
| /opt/senzing/g2/lib/libSpaceTimeBoxStandardizer.so |-|
| /opt/senzing/g2/lib/libanalytics.so |-|
| /opt/senzing/g2/lib/libboost_atomic.so |-|
| /opt/senzing/g2/lib/libboost_atomic.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_chrono.so |-|
| /opt/senzing/g2/lib/libboost_chrono.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_container.so |-|
| /opt/senzing/g2/lib/libboost_container.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_context.so |-|
| /opt/senzing/g2/lib/libboost_context.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_coroutine.so |-|
| /opt/senzing/g2/lib/libboost_coroutine.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_date_time.so |-|
| /opt/senzing/g2/lib/libboost_date_time.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_filesystem.so |-|
| /opt/senzing/g2/lib/libboost_filesystem.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_graph.so |-|
| /opt/senzing/g2/lib/libboost_graph.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_iostreams.so |-|
| /opt/senzing/g2/lib/libboost_iostreams.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_locale.so |-|
| /opt/senzing/g2/lib/libboost_locale.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_log.so |-|
| /opt/senzing/g2/lib/libboost_log.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_log_setup.so |-|
| /opt/senzing/g2/lib/libboost_log_setup.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_math_c99.so |-|
| /opt/senzing/g2/lib/libboost_math_c99.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_math_c99f.so |-|
| /opt/senzing/g2/lib/libboost_math_c99f.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_math_c99l.so |-|
| /opt/senzing/g2/lib/libboost_math_c99l.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_math_tr1.so |-|
| /opt/senzing/g2/lib/libboost_math_tr1.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_math_tr1f.so |-|
| /opt/senzing/g2/lib/libboost_math_tr1f.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_math_tr1l.so |-|
| /opt/senzing/g2/lib/libboost_math_tr1l.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_prg_exec_monitor.so |-|
| /opt/senzing/g2/lib/libboost_prg_exec_monitor.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_program_options.so |-|
| /opt/senzing/g2/lib/libboost_program_options.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_random.so |-|
| /opt/senzing/g2/lib/libboost_random.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_regex.so |-|
| /opt/senzing/g2/lib/libboost_regex.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_serialization.so |-|
| /opt/senzing/g2/lib/libboost_serialization.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_signals.so |-|
| /opt/senzing/g2/lib/libboost_signals.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_system.so |-|
| /opt/senzing/g2/lib/libboost_system.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_thread.so |-|
| /opt/senzing/g2/lib/libboost_thread.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_timer.so |-|
| /opt/senzing/g2/lib/libboost_timer.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_type_erasure.so |-|
| /opt/senzing/g2/lib/libboost_type_erasure.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_wave.so |-|
| /opt/senzing/g2/lib/libboost_wave.so.1.68.0 |-|
| /opt/senzing/g2/lib/libboost_wserialization.so |-|
| /opt/senzing/g2/lib/libboost_wserialization.so.1.68.0 |-|
| /opt/senzing/g2/lib/libdb2plugin.so |-|
| /opt/senzing/g2/lib/libeaexml2.so |-|
| /opt/senzing/g2/lib/libeaexml2.so.2 |-|
| /opt/senzing/g2/lib/libeaexml2.so.2.9.4 |-|
| /opt/senzing/g2/lib/libg2AddressComp.so |-|
| /opt/senzing/g2/lib/libg2AddressHasher.so |-|
| /opt/senzing/g2/lib/libg2ConfigParseAddr.so |-|
| /opt/senzing/g2/lib/libg2DLComp.so |-|
| /opt/senzing/g2/lib/libg2DateComp.so |-|
| /opt/senzing/g2/lib/libg2ExactDomainMatchComp.so |-|
| /opt/senzing/g2/lib/libg2ExactMatchComp.so |-|
| /opt/senzing/g2/lib/libg2FormatSSN.so |-|
| /opt/senzing/g2/lib/libg2GEOLOCComp.so |-|
| /opt/senzing/g2/lib/libg2GNRNameComp.so |-|
| /opt/senzing/g2/lib/libg2GenericHasher.so |-|
| /opt/senzing/g2/lib/libg2GroupAssociationComp.so |-|
| /opt/senzing/g2/lib/libg2IDHasher.so |-|
| /opt/senzing/g2/lib/libg2NameHasher.so |-|
| /opt/senzing/g2/lib/libg2ParseDOB.so |-|
| /opt/senzing/g2/lib/libg2ParseGEOLOC.so |-|
| /opt/senzing/g2/lib/libg2ParseID.so |-|
| /opt/senzing/g2/lib/libg2ParseName.so |-|
| /opt/senzing/g2/lib/libg2ParsePhone.so |-|
| /opt/senzing/g2/lib/libg2PartialAddresses.so |-|
| /opt/senzing/g2/lib/libg2PartialDates.so |-|
| /opt/senzing/g2/lib/libg2PartialNames.so |-|
| /opt/senzing/g2/lib/libg2PhoneComp.so |-|
| /opt/senzing/g2/lib/libg2PhoneHasher.so |-|
| /opt/senzing/g2/lib/libg2SSNComp.so |-|
| /opt/senzing/g2/lib/libg2STBHasher.so |-|
| /opt/senzing/g2/lib/libg2StrictSubsetFelems.so |-|
| /opt/senzing/g2/lib/libg2StrictSubsetNormalizedFelems.so |-|
| /opt/senzing/g2/lib/libg2StrictSubsetTokens.so |-|
| /opt/senzing/g2/lib/libg2StringComp.so |-|
| /opt/senzing/g2/lib/libicudata.so |-|
| /opt/senzing/g2/lib/libicudata.so.60 |-|
| /opt/senzing/g2/lib/libicudata.so.60.2 |-|
| /opt/senzing/g2/lib/libicui18n.so |-|
| /opt/senzing/g2/lib/libicui18n.so.60 |-|
| /opt/senzing/g2/lib/libicui18n.so.60.2 |-|
| /opt/senzing/g2/lib/libicuio.so |-|
| /opt/senzing/g2/lib/libicuio.so.60 |-|
| /opt/senzing/g2/lib/libicuio.so.60.2 |-|
| /opt/senzing/g2/lib/libicutest.so |-|
| /opt/senzing/g2/lib/libicutest.so.60 |-|
| /opt/senzing/g2/lib/libicutest.so.60.2 |-|
| /opt/senzing/g2/lib/libicutu.so |-|
| /opt/senzing/g2/lib/libicutu.so.60 |-|
| /opt/senzing/g2/lib/libicutu.so.60.2 |-|
| /opt/senzing/g2/lib/libicuuc.so |-|
| /opt/senzing/g2/lib/libicuuc.so.60 |-|
| /opt/senzing/g2/lib/libicuuc.so.60.2 |-|
| /opt/senzing/g2/lib/libmariadbplugin.so |-|
| /opt/senzing/g2/lib/libpostal.so |-|
| /opt/senzing/g2/lib/libpostal.so.1 |-|
| /opt/senzing/g2/lib/libpostal.so.1.0.0 |-|
| /opt/senzing/g2/lib/libpostgresqlplugin.so |-|
| /opt/senzing/g2/lib/libscoring.so |-|
| /opt/senzing/g2/lib/libsqliteplugin.so |-|
| /opt/senzing/g2/python/CompressedFile.py |-|
| /opt/senzing/g2/python/DumpStack.py |-|
| /opt/senzing/g2/python/G2Audit.py |-|
| /opt/senzing/g2/python/G2AuditModule.py |-|
| /opt/senzing/g2/python/G2Command.py |-|
| /opt/senzing/g2/python/G2Config.py |-|
| /opt/senzing/g2/python/G2ConfigModule.py |-|
| /opt/senzing/g2/python/G2ConfigTables.py |-|
| /opt/senzing/g2/python/G2ConfigTool.py |-|
| /opt/senzing/g2/python/G2ConfigTool.readme |-|
| /opt/senzing/g2/python/G2CreateInstance.py |-|
| /opt/senzing/g2/python/G2Database.py |-|
| /opt/senzing/g2/python/G2Diagnostic.py |-|
| /opt/senzing/g2/python/G2Engine.py |-|
| /opt/senzing/g2/python/G2Exception.py |-|
| /opt/senzing/g2/python/G2Export.py |-|
| /opt/senzing/g2/python/G2Hasher.py |-|
| /opt/senzing/g2/python/G2HasherModule.py |-|
| /opt/senzing/g2/python/G2Loader.py |-|
| /opt/senzing/g2/python/G2Module.ini | /etc/opt/senzing/G2Module.ini |We have two G2Module.ini currently, one in data and one in python. this would consoldate into on in etc|
| /opt/senzing/g2/python/G2Module.py |-|
| /opt/senzing/g2/python/G2Product.py |-|
| /opt/senzing/g2/python/G2ProductModule.py |-|
| /opt/senzing/g2/python/G2Project.ini | We have two G2Project.ini currently, one in data and one in python. this would consoldate into on in etc |
| /opt/senzing/g2/python/G2Project.py |-|
| /opt/senzing/g2/python/G2S3.py |-|
| /opt/senzing/g2/python/demo/ofac/cust.json |/var/opt/senzing/g2/python/demo/ofac/cust.json | (or etc since they could be demo config files?) |
| /opt/senzing/g2/python/demo/ofac/ofac.json |/var/opt/senzing/g2/python/demo/ofac/ofac.json | (or etc since they could be demo config files?) |
| /opt/senzing/g2/python/demo/ofac/project.json | /var/opt/senzing/g2/python/demo/ofac/project.json | (or etc since they could be demo config files?) |
| /opt/senzing/g2/python/demo/sample/project.csv | /var/opt/senzing/g2/python/demo/sample/project.csv | (or etc since they could be demo config files?) |
| /opt/senzing/g2/python/demo/sample/project.json | /var/opt/senzing/g2/python/demo/sample/project.json | (or etc since they could be demo config files?) |
| /opt/senzing/g2/python/demo/sample/sample_company.csv | /var/opt/senzing/g2/python/demo/sample/sample_company.csv | (or etc since they could be demo config files?) |
| /opt/senzing/g2/python/demo/sample/sample_company.json | /var/opt/senzing/g2/python/demo/sample/sample_company.json | (or etc since they could be demo config files?) |
| /opt/senzing/g2/python/demo/sample/sample_person.csv | /var/opt/senzing/g2/python/demo/sample/sample_person.csv | (or etc since they could be demo config files?) |
| /opt/senzing/g2/python/demo/sample/sample_person.json | /var/opt/senzing/g2/python/demo/sample/sample_person.json | (or etc since they could be demo config files?) |
| /opt/senzing/g2/python/g2config.json | /etc/opt/senzing/g2config.json | We have two g2config.json currently, one in data and one in python. this would consoldate into on in etc |
| /opt/senzing/g2/python/g2purge.umf |-|
| /opt/senzing/g2/python/g2silent.cfg | /etc/opt/senzing/g2silent.cfg | This doesn't exist in data, only in python. Moving it to etc would make it product wide. Is that ok? |
| /opt/senzing/g2/sdk/c/g2PluginInterface.h |-|
| /opt/senzing/g2/sdk/c/libg2.h |-|
| /opt/senzing/g2/sdk/c/libg2audit.h |-|
| /opt/senzing/g2/sdk/c/libg2config.h |-|
| /opt/senzing/g2/sdk/c/libg2diagnostic.h |-|
| /opt/senzing/g2/sdk/c/libg2hasher.h |-|
| /opt/senzing/g2/sdk/c/libg2product.h |-|
| /opt/senzing/g2/sdk/c/libg2ssadm.h |-|
| /opt/senzing/g2/sdk/java/com/senzing/g2/engine/G2Audit.java |-|
| /opt/senzing/g2/sdk/java/com/senzing/g2/engine/G2AuditJNI.java |-|
| /opt/senzing/g2/sdk/java/com/senzing/g2/engine/G2Config.java |-|
| /opt/senzing/g2/sdk/java/com/senzing/g2/engine/G2ConfigJNI.java |-|
| /opt/senzing/g2/sdk/java/com/senzing/g2/engine/G2Diagnostic.java |-|
| /opt/senzing/g2/sdk/java/com/senzing/g2/engine/G2DiagnosticJNI.java |-|
| /opt/senzing/g2/sdk/java/com/senzing/g2/engine/G2Engine.java |-|
| /opt/senzing/g2/sdk/java/com/senzing/g2/engine/G2Fallible.java |-|
| /opt/senzing/g2/sdk/java/com/senzing/g2/engine/G2JNI.java |-|
| /opt/senzing/g2/sdk/java/com/senzing/g2/engine/G2Product.java |-|
| /opt/senzing/g2/sdk/java/com/senzing/g2/engine/G2ProductJNI.java |-|
| /opt/senzing/g2/sdk/java/com/senzing/g2/engine/Result.java |-|
| /opt/senzing/g2/sdk/python/G2Audit.py |-|
| /opt/senzing/g2/sdk/python/G2Config.py |-|
| /opt/senzing/g2/sdk/python/G2Diagnostic.py |-|
| /opt/senzing/g2/sdk/python/G2Engine.py |-|
| /opt/senzing/g2/sdk/python/G2Exception.py |-|
| /opt/senzing/g2/sdk/python/G2Product.py |-|
| /opt/senzing/g2/sdk/python/old/G2AuditModule.py |-|
| /opt/senzing/g2/sdk/python/old/G2ConfigModule.py |-|
| /opt/senzing/g2/sdk/python/old/G2Exception.py |-|
| /opt/senzing/g2/sdk/python/old/G2Module.py |-|
| /opt/senzing/g2/sdk/python/old/G2ProductModule.py |-|
| /opt/senzing/g2/sdk/streams/G2CommonToolkit.tgz |-|
| /opt/senzing/g2/setupEnv |-|
| /opt/senzing/g2/sqldb/G2C.db | /var/opt/lib/senzing/sqlite/G2C.db | This also exists in data should it? |
| /opt/senzing/g2/util/NewReleaseCheck.sh | /opt/senzing/g2/NewReleaseCheck.sh |

