# 创建多个数据点（多个传感器）Create Multiple Data Points For Multi-Sensors

## POST

    /v1.1/device/<device_id>/datapoints

## POST数据

    [
      {"sensor_id": <sensor_id>, "value": 50},//数值型
      {"sensor_id": <sensor_id>, "value": {"lat":35.4567,"lng":46.1234,"speed":98.2, offset: true}}，//GPS型
      {"sensor_id": <sensor_id>, "value": {/*your code here*/}}，//泛型
    ]

***注意*：不支持图片型和微博型传感器**

## 访问授权

    U-ApiKey: <your_api_key>

## 返回值

    {"<sensor_id>":"","<sensor_id>":""}
