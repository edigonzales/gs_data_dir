# gs_data_dir

```
java -jar /Users/stefan/apps/ili2pg-4.4.6/ili2pg-4.4.6.jar --dbhost localhost --dbport 54321 --dbdatabase edit --dbusr admin --dbpwd admin \
--dbschema arp_npl --models SO_Nutzungsplanung_Publikation_20190909 \
--defaultSrsCode 2056 --createGeomIdx --createFk --createFkIdx --createUnique --createEnumTabs --beautifyEnumDispName --createMetaInfo --createNumChecks --nameByTopic --strokeArcs \
--disableValidation \
--doSchemaImport --import /Users/stefan/Downloads/ch.so.arp.nutzungsplanung_xtf/ch.so.arp.nutzungsplanung.xtf
```

```
java -jar /Users/stefan/apps/ili2pg-4.4.6/ili2pg-4.4.6.jar --dbhost localhost --dbport 54322 --dbdatabase pub --dbusr admin --dbpwd admin \
--dbschema arp_richtplan_pub --models SO_ARP_Richtplan_Publikation_20210210 \
--defaultSrsCode 2056 --createGeomIdx --createFk --createFkIdx --createUnique --createEnumTabs --beautifyEnumDispName --createMetaInfo --createNumChecks --nameByTopic --strokeArcs \
--disableValidation \
--doSchemaImport --import /Users/stefan/Downloads/ch.so.arp.richtplan_xtf/ch.so.arp.richtplan.xtf
```

```
java -jar /Users/stefan/apps/ili2pg-4.4.6/ili2pg-4.4.6.jar --dbhost localhost --dbport 54322 --dbdatabase pub --dbusr admin --dbpwd admin \
--dbschema arp_gewaesserschutz_pub --models SO_AfU_Gewaesserschutz_Publikation_20210303 \
--defaultSrsCode 2056 --createGeomIdx --createFk --createFkIdx --createUnique --createEnumTabs --beautifyEnumDispName --createMetaInfo --createNumChecks --nameByTopic --strokeArcs \
--disableValidation \
--doSchemaImport --import /Users/stefan/Downloads/ch.so.afu.gewaesserschutz_xtf/ch.so.afu.gewaesserschutz.xtf
```



```
export GEOSERVER_DATA_DIR=/Users/stefan/sources/gs_data_dir/data_dir_alpha
./startup.sh
```

