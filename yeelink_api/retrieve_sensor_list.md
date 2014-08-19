# 获取传感器列表 Retrieve Sensor List

## GET

    /v1.1/device/<device_id>/sensors

## 返回值

该设备的所有传感器列表信息

**JOSN**


    [
      {
        "id": 2,
        "title": "test2",
        "about": "just a test",
        "type":0,
        "last_update": 1380009649,
        "last_data":"317",
        "last_data_gen":null
      },
      {
        "id": 3,
        "title": "test3",
        "about": "just a test",
        "type":6,
        "last_update": 1380009669,
        "last_data":null;,
        "last_data_gen":{"lat":23.8,"lng":54.5,"speed":45}
      }
    ]

| 字段 | 类型 | 可为空 | 备注 |
| -- | -- | -- | -- |
| title | string | 否 | 标题 |
| about | string | 否 | 简介 |
| tags | string | 否 | 标签 |

##访问授权

    U-ApiKey: <your_api_key>
