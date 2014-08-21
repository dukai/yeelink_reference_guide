# 获取数据点 Retrieve Data Point

## GET

    /v1.1/device/<device_id>/sensor/<sensor_id>/datapoint/<key>
## 返回值

### key不为空

    //数值型
    {
      "value": 39.4
    }
    //GPS型
    {
     "value": {"lat":35.4321,"lng":46.3451,"speed":98.2}
    }
    //泛型
    {
     "value": {...}
    }
    //微博型
    {
      "status_cnt":0,"follower_cnt":0,"msg_cnt":0
    }
### key为空

    //数值型
    {
      "timestamp":"2012-03-15T16:13:14",
      "value": 39.4,
      "sensor_id": 2132,
      "device_id": 2234
    }
    //GPS型
    {
      "timestamp":"2012-03-15T16:13:14",
      "value": {"lat":35.4321,"lng":46.3451,"speed":98.2}
    }
    //泛型
    {
      "key":"e10adc3949ba59abbe56e037f20f884e",
      "value": {...}
    }

## 访问授权

    U-ApiKey: <your_api_key>
