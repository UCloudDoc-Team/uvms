<!--一下子提供一种思路，欢迎大家发挥 -->

# 快速入门

![快速入门.png](images/快速入门.png)


## 1.注册并登陆UCloud账号

* 注册UCloud账号：[点击快速注册](https://passport.ucloud.cn/#login)或直接联系您的客户经理


## 2.完成企业实名制认证

* 企业实名认证：[点击账号实名认证](https://passport.ucloud.cn/login?service=https%3A%2F%2Fconsole.ucloud.cn%2Fuaccount%2Fauthentication#login)，可联系您的客户经理查看进度。


## 3.开通语音消息服务

* 勾选我已阅读并同意[UCloud语音消息服务协议](/uvms/introduction/agreement.md)，免费开通语音消息服务；勾选同意后，才可以进行企业资质认证。


## 4.创建企业完成资质审核

根据基础运营商的管控要求，使用语音线路和申请号码需提交相关企业资质材料，企业资质审核通过后您才可以正式使用语音消息服务。

* [点击创建企业](https://console.ucloud.cn/uvms/company/create)，按要求准备相关材料并上传。


## 5.添加应用（按需）

除内部生产告警场景外，其他使用场景均需添加应用，应用指的是您需要使用语音消息服务的产品，如APP/网站/小程序/公众号等，应用审核通过后才可以创建语音模板。

* [点击创建应用](https://console.ucloud.cn/uvms/qualification)，按要求上传相关材料。


## 6.创建模板

语音模板支持两种类型：文本模板及音频模板，文本模板可通过TTS转换成音频进行播报，音频模板为您提前录制好的固定音频内容。在发起语音呼叫请求时，调用对应的模板ID及变量来实现语音呼叫，因此您需要在发起请求前，创建好语音模板并通过审核，才可以正常使用。

* [点击创建模板](https://console.ucloud.cn/uvms/interval)


## 7.购买语音套餐包

已完成企业实名认证及企业资质认证的账号可购买语音套餐包，特别注意的是专享号码套餐包需申请专享号码配套使用，随机号码套餐包与专享号码套餐包不通用。

* [立即购买语音套餐包](https://console.ucloud.cn/uvms/buy?Purpose=1)

## 8.申请号码（按需）

如您对号码外显、号码归属地等有特殊要求，如需要靓号、95号、指定号码作为主叫号码等，您需要申请专享号码。

* [点击申请号码](https://console.ucloud.cn/uvms/interval)


## 9.语音呼叫

您可通过语音消息服务控制台或调用发送API/SDK，发起语音呼叫请求，对被叫号码进行语音模板播报。

* 登陆语音消息服务控制台：[语音消息服务控制台](https://console.ucloud.cn/uvms/new)
* 对接发送API或SDK：[API文档](https://docs.ucloud.cn/api/uvms-api/send_uvms_message)、[SDK文档]()


## 10.查询回执

查询回执状态、查询数据统计等信息，支持如下几种方式：

* 控制台查询：[点击查询](https://console.ucloud.cn/uvms/)
* 对接状态报告查询API或SDK查询：[API文档](https://docs.ucloud.cn/api/uvms-api/send_uvms_message)、[SDK文档]()
* 配置回调地址：[点击配置](https://console.ucloud.cn/uvms/config)
