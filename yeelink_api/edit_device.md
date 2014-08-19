# 编辑设备

## PUT

    /v1.1/devices/<device_id>

## PUT数据

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

## 返回值

    返回值为空

## 访问授权

    U-ApiKey: <your_api_key>
    P-ApiKey: <product_api_key>
