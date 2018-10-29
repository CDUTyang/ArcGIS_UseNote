## ArcMap创建SQLite地理数据库
ArcMap没有提供直接创建SQLite数据库的功能，只能通过Python窗口写ArcPy代码创建SQLite。

> ST_GEOMETRY——ESRI 公司的空间存储类型。这是默认的。  
  SPATIALITE——spatialite 空间存储类型。  
  GEOPACKAGE——OGC geopackage geopackage。

``` py
arcpy.gp.CreateSQLiteDatabase("sqlite_database_path.sqlite", "ST_GEOMETRY")
arcpy.gp.CreateSQLiteDatabase("sqlite_database_path.gpkg", "GEOPACKAGE")
```
