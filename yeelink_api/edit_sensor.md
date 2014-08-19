# Edit Sensor

##PUT

    /v1.1/device/<device_id>/sensor/<sensor_id>

PUT数据

    {
      "title":"温度传感器测试",
      "about":"这是一个测试传感器",
      "tags":"数据,温度",
      "unit": {
         "name": "摄氏度",
         "symbol": "°C"
       }
    }


| 字段 | 类型 | 可为空 | 备注 |
| -- | -- | -- | -- |
| type | string | 否 | 传感器类型：value, switcher, gps, gen, photo |
| title | string | 否 | 标题 |
| about | string | 否 | 简介 |
| tags | string | 否 | 标签 |
| unit | json | 否 | 单位符号 |
| unit.name | string | 否 | 单位 |
| unit.symbol | string | 否 | 符号 |

##返回值

    返回值为空

##访问授权

    U-ApiKey: <your_api_key>
