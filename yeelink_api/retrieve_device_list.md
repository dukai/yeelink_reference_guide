# 获取设备列表

## GET

    /v1.1/devices

## 返回值

**JSON**

    [
      {
        "id": "2",
        "title": "test2",
        "about": "just a test"
      },
      {
        "id": "3",
        "title": "test3",
        "about": "just a test"
      }
    ]

返回值为一个JSON数组，数组内容为用户所有的设备列表

| 字段 | 类型 | 备注 |
| -- | -- | -- |
| id | int | 设备ID |
| title | string | 设备标题 |
| about | string | 设备简介 |

## 访问授权

    U-ApiKey: <your_api_key>
    P-ApiKey: <product_api_key>
