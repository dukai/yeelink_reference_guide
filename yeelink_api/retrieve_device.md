# 获取设备信息

##GET

    /v1.1/devices/<device_id>

## 返回值

**JSON**

    {
      "title": "test3",
      "about": "just a test",
      "tags": "lab",
      "local": "Qingdao",
      "latitude": 0.444,
      "longitude": 0.555
    }


| 字段 | 类型 | 可为空 | 备注 |
| -- | -- | -- | -- |
| title | string | 否 | 标题 |
| about | string | 否 | 简介 |
| tags | string | 否 | 标签 |
| local | string | 否 | 地理位置，如：山东青岛 |
| latitude | float | 否 | 经度 |
| longitude	 | float | 否 | 纬度 |

## 访问授权

    //开发者访问
    U-ApiKey: <your_api_key>
    //产品设备访问
    P-ApiKey: <your_api_key>
