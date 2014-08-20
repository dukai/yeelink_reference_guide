# Feedback

终端设备反馈产品意见

##POST

    /v1.1/product/feed/<product_sn>

##POST内容

    {
      “message”: “your client user feed back message”
    }

|字段|	 类型|	 备注|
|--|--|--|
|message|	 string	| 用户反馈的意见|

##授权方式

    P-ApiKey: <your_api_key>
##返回值

返回值为空
