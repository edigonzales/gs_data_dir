```
gdal_retile.py -v -r bilinear -levels 6 -ps 2048 2048 -s_srs EPSG:2056 -co "TILED=YES" -co "COMPRESS=JPEG" -targetDir geoserver/ch.so.agi.orthofoto_2006.rgb/ geodata/ch.so.agi.orthofoto_2006.rgb/orthofoto_2006_rgb_12_5cm.vrt
```
```
ls -a geodata/ch.so.agi.orthofoto_2006.rgb/*12_5cm.tif > foo.txt

gdal_retile.py -v -r bilinear -levels 6 -ps 2048 2048 -s_srs EPSG:2056 -co "TILED=YES" -co "COMPRESS=JPEG" -targetDir geoserver/foo/ --optfile foo.txt
```

Variante 2 führt zu Fehlern. gdal_retile erwartet wohl Files, die es so nicht gibt:

```
geoserver/foo/25921227_12_5cm_137_019.tif : 36864|278528-->2048-1472
geoserver/foo/25921227_12_5cm_137_020.tif : 38912|278528-->2048-1472
ERROR 4: geoserver/foo/25921227_12_5cm_001_001.tif: No such file or directory
Error opening: <class 'NameError'>
```