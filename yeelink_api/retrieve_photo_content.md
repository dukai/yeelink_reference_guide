# 获取图片内容 Retrieve Photo Content

通过本接口可以获取图片的二进制内容。

## GET

    /v1.1/device/<device_id>/sensor/<sensor_id>/photo/content/<key>

key可为空，当key为空时返回最新一条数据

## 返回值

图片的二进制内容

## 访问授权

    U-ApiKey: <YOUR_API_KEY_HERE>
