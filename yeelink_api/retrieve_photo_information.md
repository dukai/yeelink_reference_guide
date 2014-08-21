# 获取图片信息 Retrieve Photo Information

通过本接口可以获取图片的相关信息，比如尺寸，大小，类型和地址等。

## GET

    /v1.1/device/<device_id>/sensor/<sensor_id>/photo/info/<key>

key可为空，当key为空时返回最新一条数据

##返回值

**JSON**

    {
      "value":{
        "size": 45, "width": 240, "height": 320, "type": "jpg", "url":"xxxx"
      }
    }
## 访问授权

    U-ApiKey: <YOUR_API_KEY_HERE>
