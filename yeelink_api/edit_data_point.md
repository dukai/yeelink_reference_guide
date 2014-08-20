# Edit Data Point

## PUT

    /v1.1/device/<device_id>/sensor/<sensor_id>/datapoint/<key>

## PUT数据

### 数值型传感器

    {
      "value": 39.4
    }
### GPS型传感器

    {
      "value": {"lat":35.4321,"lng":46.3451,"speed":98.2}
    }
### 泛型传感器[编辑]
    {
      "value": {...}
    }
## 返回值

空
