## 请求说明
请求为 JSON Object 格式。
### 请求参数

```json
{
    "TaskNo": "d0****f7-0fc3-****-****-9f73****6c6e",
    "Phone": "185****9057",
    "ShowNumber": "021****9057",
    "CostCount": 2,
    "ReceiptResult": 1, 
    "ReceiptCode": "Delivrd",
    "ReceiptDesc": "用户接收成功",
    "CallStartTime": 1649756907000,
    "AnswerTime": 1649756907000,
    "CallEndTime": 1649756907000,
    "Duration": 23,
    "UserId": "you man c define the content by yrself"
}
```

### 参数说明

| Parameter name | Type   | Description                                                                                                                | Case             | Required |
| -------------- | ------ | -------------------------------------------------------------------------------------------------------------------------- | ---------------- | -------- |
| TaskNo         | string | [发送语音消息](https://docs.ucloud.cn/api/uvms-api/send_uvms_message) 的发送序列号                                         | xddd-xx-ss-ss-ss | Y        |
| ShowNumber     | string | 主叫号码                                                                                                                   | 18512345678      | Y        |
| Phone          | string | 被叫号码                                                                                                                   | 18512345678      | Y        |
| CostCount      | int    | 通知消耗（条或分钟）                                                                                                       | 2                | Y        |
| ReceiptResult  | int    | 回执状态结果，可根据该字段判断发送结果，枚举值> 1：代表短消息发送成功 > 2：代表短消息发送失败> 3：代表运营商未上报状态报告 | 1                | Y        |
| ReceiptCode    | string | 状态报告编码                                                                                                               | Delivrd          | Y        |
| ReceiptDesc    | string | 状态报告说明                                                                                                               | 用户接收成功     | Y        |
| CallStartTime  | int    | 呼叫开始时间 （毫秒时间戳）                                                                                                | 1649756907000    | Y        |
| AnswerTime     | int    | 接听电话时间（毫秒时间戳）                                                                                                 | 1649756907000    | Y        |
| CallEndTime    | int    | 呼叫结束时间 （毫秒时间戳）                                                                                                | 1649756907000    | Y        |
| Duration       | int    | 呼叫用时（秒）                                                                                                             | 32               | Y        |
| UserId         | string | 自定义的业务标识ID，字符串（ 长度不能超过32 位），不支持 单引号、表情包符号等特殊字符                                      | ucloud-uhost-001 | N        |

## 响应说明
### 响应示例
``` json
{
    code: 0,
    message: "ok"
}
```


### 参数说明
| code | message | Description |
| ---- | ------- | ----------- |
| 0    | ok      | 接受成功    |


## 重推说明

首次推送失败后（响应http code 不是200），将每隔1秒进行重推，累计重推3次仍未成功，将停止推送。


