# 获取历史数据 Retrieve History Data

## GET

    /v1.1/device/<device_id>/sensor/<sensor_id>.json?start=<start_timestamp>&end=<end_timestamp>&interval=<interval>&page=<page>

| 字段 | 类型 | 备注 |
| -- | -- | -- |
| device_id | int | 设备ID |
| sensor_id | int | 传感器ID |
| start_timestamp | string | 开始时间，格式：2014-5-10T11：40 |
| end_timestamp | string | 开始时间，格式：2014-5-15T11：40 |
| interval | int | 间隔时间 |
| page | int | 分页，默认是1 |


interval（数据采样间隔）说明

|Interval | 说明 |
| -- | -- |
|1	| 每秒|
|10	| 10秒|

##返回值[编辑]
**JSON**

### 数值型传感器[编辑]

    [
      {"timestamp": "2012-06-15T14:00:00", "value":315},
      {"timestamp": "2012-06-15T14:00:10", "value":316},
      {"timestamp": "2012-06-15T14:00:20", "value":317},
      {"timestamp": "2012-06-15T14:00:30", "value":317},
      {"timestamp": "2012-06-15T14:00:40", "value":317}
    ]

### GPS型传感器[编辑]

    [
      {"timestamp": "2012-06-15T14:00:00", "value":{"lat":35.4,"lng":46.1,"speed":98.2}},
      {"timestamp": "2012-06-15T14:00:10", "value":{"lat":34.1,"lng":76.3,"speed":78.9}},
      {"timestamp": "2012-06-15T14:00:20", "value":{"lat":36.6,"lng":56.1,"speed":99.3}},
      {"timestamp": "2012-06-15T14:00:30", "value":{"lat":33.4,"lng":46.34,"speed":120}},
      {"timestamp": "2012-06-15T14:00:40", "value":{"lat":35.4,"lng":46.1,"speed":98.2}}
    ]

### 泛型传感器[编辑]

    [
        {"key": "custome key", "value": {
            "custom_key": "custom content"
        }}
    ]

### 图片型传感器[编辑]

    [
      {"timestamp": "2012-03-15T16:13:14", "value":{"size":45,"width":240,"height":320,"type":"jpg", url: ''},
      {"timestamp": "2012-03-15T16:13:24", "value":{"size":180,"width":100,"height":320,"type":"png", url: ''},
      {"timestamp": "2012-03-15T16:13:34", "value":{"size":1024,"width":480,"height":360,"type":"gif", url: ''},
      {"timestamp": "2012-03-15T16:13:44", "value":{"size":2000,"width":240,"height":320,"type":"jpg", url: ''},
    ]

## 访问授权

    U-ApiKey: <your_api_key>
    P-ApiKey: <your_api_key>
