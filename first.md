

主要分两个坐标系统：
 * Geographic coordinate system(地理坐标系)
 * projected coordinate system(投影坐标系)

投影坐标系中投影方式有很多。
 * UTM：
 * Web墨卡托：正方形，南北会拉伸，非等角，在线地图广泛使用。

空间参照系统：SRS，spatial reference system,WKT 表示，里面有投影，椭球，基准

空间参照标识符：SRID，指代一直SRS
每一个数据都应该指定SRID，比如4326，代表WGS84
