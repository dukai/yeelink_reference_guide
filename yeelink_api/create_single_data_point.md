# create single data point

为传感器创建一个数据点

## POST

    /v1.1/device/<device_id>/sensor/<sensor_id>/datapoints

## POST数据

### 数值型传感器

    {
      "timestamp":"2012-03-15T16:13:14",
      "value":294.34
    }

| 字段 | 类型 | 可为空 | 备注 |
| -- | -- | -- | -- |
| timestamp | string | 否 | 时间，可为空，本值为空时会自动生成当前时间 |
| value | float | 否 | 值 |

### GPS型传感器

    {
      "timestamp":"2012-03-15T16:13:14",
      "value":{"lat":35.4567,"lng":46.1234,"speed":98.2, offset: true}
    }

| 字段 | 类型 | 可为空 | 备注 |
| -- | -- | -- | -- |
| timestamp | string | 否 | 时间，可为空，本值为空时会自动生成当前时间 |
| value | json | 否 | 由多个参数组成的json对象 |
| value.lat | float | 否 | 纬度 |
| value.lng | float | 否 | 经度 |
| value.speed | float | 否 | 速度 |
| value.offset | float | 否 | 偏移 |

### 泛型传感器

    {
       "key":"e10adc3949ba59abbe56e037f20f884e",
       "value":{
            "custom_key_one": "your custom content",
            "custom_key_two": "your custom content"
       }
    }

| 字段 | 类型 | 可为空 | 备注 |
| -- | -- | -- | -- |
| key | string | 否 | 键值，长度不超过128个字符 |
| value | json | 否 | 自定义数据格式，长度不超过1024个字符 |

图片传感器[编辑]
图片的二进制内容
返回值[编辑]
返回值为空

## 访问授权

    U-ApiKey: <your_api_key>
