# create multiple data points for one sensor

对同一传感器同时上传多个数据点。

## POST

    /v1.1/device/<device_id>/sensor/<sensor_id>/datapoints
### 数值型传感器

    [
      {
        "timestamp":"2012-03-15T16:13:14",
        "value":294.34
      },
      {
        "timestamp":"2012-03-15T16:13:24",
        "value":284.34
      }
    ]
### GPS型传感器

    [
      {
        "timestamp":"2012-03-15T16:13:14",
        "value":{"lat":35.4567,"lng":46.1234,"speed":98.2}
      },
      {
        "timestamp":"2012-03-15T16:13:24",
        "value":{"lat":35.4567,"lng":46.1234,"speed":98.2}
      }
    ]

### 泛型传感器

    [
      {
      "key":"bbbbbbbbbbbbbbbbbbbbbbbbbbbbbb",
        "value":{
          //your code here
        }
      },
      {
      "key":"aaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
        "value":{
          //your code here
        }
      },
    ]
## 访问授权

    U-ApiKey: <your_api_key>
## 返回值

返回值为空
