# 绑定产品 Bind Product

绑定并激活产品终端设备

##POST

    /v1.1/product/bind/<product_sn>
##POST内容

    {
      “user_login”: “yourname”,
      “force”: true
    }

|字段| 类型| 备注|
|--|--|--|
|user_login	| string	| 用户登录名|
|force	| boolean|	 是否为强制（可选项）|

##授权方式

    P-ApiKey: <your_api_key>

##返回值

返回值为空
