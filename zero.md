参考: https://live.osgeo.org/zh/quickstart/geoserver_quickstart.html

GeoServer是基于Java的，它的github topic说明了它涉及的东西：
* web 是作为web服务的
* mapping 测绘，绘图
* web-mapping 网络化地图
* java 使用Java开发
* wms 发布成wms服务
* wfs 同理
* wps 同理
* wcs 同理
* maps 多种地图服务


geoserver的工作流程是：
导入数据 --> 配置、发布图层. 

可选图层样式编辑，对地图样式编辑以满足用户的需求。

可建图层组，就是将多个图层组合管理，像一个图层一样使用。用户编辑样式可以自定义地图风格。

底层数据几乎支持所有的公开数据格式。


接下来的部分主要是参考资源里面的书。

空间数据如何存储和如何发布为地图的。

底层数据也支持postgis, oracle, mysql.

图层风格自定义，使用sld

>SLD是风格化图层描述器（Styled Layer Descriptor）的简称，是2005年OGC提出的一个标准，这个标准在一定条件下允许WMS服务器对地图可视化的表现形式进行扩展。在没有SLD之前，只能使用一些已经在服务器上规定好的样式来对地图进行可视化。而当使用了实现了SLD标准之后，它允许我们从客户端来对地图进行定义自己的样式，分级显示等操作，极大的扩展了地图可视化的灵活性。
>参考：https://www.cnblogs.com/naaoveGIS/p/4176198.html

支持GeoWebCache

通过rest interface control the GeoServer configuration.
这样就支持远端配置，比如用户自定义图层样式。

security module

支持多用户登录。
