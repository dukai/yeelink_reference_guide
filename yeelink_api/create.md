# 创建设备

本资源用于创建一个yeelink开发设备。

## POST

    v1.1/devices

## POST 数据

    {
      "title":"test",
      "about":"test api",
      "tags":"temperature,lab",
      "location":{
        "local":"Qingdao",
        "latitude":0.444,
        "longitude":0.555
      }
    }

| 字段 | 类型 | 可为空 | 备注 |
| -- | -- | -- | -- |
| title | string | 否 | 标题 |
| about | string | 否 | 简介 |
| tags | string | 否 | 标签 |
| location | json | 否 | 地理位置信息 |
| location.local | string | 否 | 地理位置，如：山东青岛 |
| location.latitude | float | 否 | 经度 |
| location.longitude	 | float | 否 | 纬度 |

##返回值

**JSON**

    {
      "device_id": 2
    }

##访问授权

    U-ApiKey: <your_api_key>

本接口目前不支持产品设备访问。
