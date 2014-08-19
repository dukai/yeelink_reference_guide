# 获取传感器 Retrieve Sensor

对该地址发起GET请求将会获得指定ID的传感器的详细信息。

## GET

    /v1.1/device/<device_id>/sensor/<sensor_id>
##返回值

该设备的详细信息

**JOSN**

### 数值型传感器

    {
      "title":"test",
      "about":"just a test",
      "tags":"tag1,tag2",
      "unit_name": "temperature",
      "unit_symbol": "C"
    }


| 字段 | 类型 | 可为空 | 备注 |
| -- | -- | -- | -- |
| title | string | 否 | 标题 |
| about | string | 否 | 简介 |
| tags | string | 否 | 标签 |
| unit_name | string | 否 | 单位 |
| unit_symbol | string | 否 | 符号 |


### GPS传感器

    {
      "title":"test",
      "about":"just a test",
      "tags":"tag1,tag2"
    }

| 字段 | 类型 | 可为空 | 备注 |
| -- | -- | -- | -- |
| title | string | 否 | 标题 |
| about | string | 否 | 简介 |
| tags | string | 否 | 标签 |

### 泛型传感器

    {
      "title":"test",
      "about":"just a test",
      "tags":"tag1,tag2"
    }

| 字段 | 类型 | 可为空 | 备注 |
| -- | -- | -- | -- |
| title | string | 否 | 标题 |
| about | string | 否 | 简介 |
| tags | string | 否 | 标签 |

### 图像传感器

    {
      "title":"test",
      "about":"just a test",
      "tags":"tag1,tag2"
    }

| 字段 | 类型 | 可为空 | 备注 |
| -- | -- | -- | -- |
| title | string | 否 | 标题 |
| about | string | 否 | 简介 |
| tags | string | 否 | 标签 |

## 访问授权

    U-ApiKey: <your_api_key>
