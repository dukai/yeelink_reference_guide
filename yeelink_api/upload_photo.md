# Upload Photo

对该URL的一个HTTP POST请求会为指定的图像传感器上传一幅新的图像, 使用此API来为图像传感器存储图像数据, 目前只支持上传jpg, png, gif类型的图像.

## POST

    /v1.1/device/<device_id>/sensor/<sensor_id>/photos
## POST内容

图片的二进制内容

## 返回值

返回值为空

## 访问授权

    U-ApiKey: <your_api_key>
