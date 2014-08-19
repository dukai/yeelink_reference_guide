# API约定

本部分包含API的默认约定。

## 返回的status code

| code | 信息 | 备注 |
| -- | -- | -- |
| 200 | 执行成功 | 创建或者更新等操作成功 |
| 403 | 权限不足 | &nbsp; |
| 404 | 访问的资源不存在 | &nbsp; |
| 406 | 数据格式错误 | &nbsp; |
| 500 | 服务器内部错误 | &nbsp; |

# 数据格式

数据创建获取时使用的数据格式为JSON，相关JSON的内容请参见[JSON](http://json.org)。

请注意，JSON中的数值规范与C或者Java中的数值非常类似，但是在编码细节有细微不同，并且没有八进制和十六进制格式。下图是JSON中的数值格式规范。

![](http://wiki.yeelink.net/images/4/46/Number.gif)

    //以下格式是正确格式
    {value: 1}
    {value: 1.1}
    {value: -1}
    {value: 0}
    {value: 0.1}
    {value: 0.10} //实际保存中保存0.1

    //以下格式为错误格式
    {value: 0.00}
    {value: -0.00}
    {value: 0x1}
    {value: 01}

如果服务器返回406请检查是否因为格式错误导致服务器拒绝访问。
