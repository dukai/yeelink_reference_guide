# 获取产品信息 Retrieve Product Information

查看产品设备的信息

##GET

    /v1.1/product/<product_sn>
##授权方式

    P-ApiKey: <your_api_key>
##返回值

**JSON**

    {
      "id":9246,
      "title":"\u7cfb\u7edf\u6027\u80fd\u76d1\u6d4b",
      "about":"\u7cfb\u7edf\u6027\u80fd\u76d1\u6d4b",
      "tags":"\u7cfb\u7edf",
      "local":"\u5c71\u4e1c \u9752\u5c9b\u5e02 ",
      "latitude":"36.08011251333357",
      "longitude":"120.3953504562378"
    }

|id	| 类型|	 备注|
|--|--|--|
|id	| int|	 设备ID |
|title	| string|	 标题|
|about	| string|	 关于|
|tags	| string|	 标签|
|local	| string|	 地理信息|
|latitude|	 float	| 维度|
|longitude	| float	| 经度|
