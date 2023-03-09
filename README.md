# APISpace 介绍
**本 API 服务由 [APISpace（apispace.com）](https://www.apispace.com/?utm_source=github&utm_term=yanzhengmaduanxin) 提供。**

APISpace 是 Eolink 旗下专业的 API 开放与交易平台，为广大企业以及个人开发者提供多维度、全方位的API接口，覆盖短信验证、天气查询、快递物流、OCR文字识别等海量 API 服务，帮助用户快速获取数据，降低获取数据的成本和难度，提升开发效率。

APISpace 提供15种开发语言的代码示例，分别是：
- Java(OK HTTP)
- HTTP
- cURL
- 微信小程序
- PHP(pecl_http)、PHP(cURL)
- Python(http.client)、Python(Requests)
- JavaScript(Jquery AJAX)、JavaScript(XHR)
- NodeJS(Native)、NodeJS(Request)
- Ruby(Net:Http)
- Shell(Httpie)、Shell(cUrl)

# 验证码短信
支持三大运营商，虚拟运营商短信发送，电信级运维保障，独享专用通道，3秒可达，99.99％到达率，支持大容量高并发。

**使用该产品前，您需要通过 [https://www.apispace.com/eolink/api/sms-code/introduction](https://www.apispace.com/eolink/api/sms-code/introduction?utm_source=github&utm_term=yanzhengmaduanxin) 申请API服务**

本文档末尾提供了 Python(Requests) 的调用代码示例，可以前往文档末尾查看。

更多代码示例：[https://www.apispace.com/eolink/api/sms-code/guidence/](https://www.apispace.com/eolink/api/sms-code/guidence/?utm_source=github&utm_term=yanzhengmaduanxin)

### 使用须知

1.  **验证码短信** 支持批量发送给多个号码，按照 **号码个数** 以及 **短信长度** 扣除实际请求次数，70字内算一条。
1.  验证码短信需要进行 **企业认证后** 才可以使用，提交企业认证后会有相关工作人员联系审核。审核后工作人员会帮您进行模板提交等操作。

### 产品优势

-   **三网合一**：联手三大运营商，三网短信通道落地，还支持虚拟运营商号段。

<!---->

-   **多通道备份**：智能切换短信通道，保证短信发送不间断。

<!---->

-   **独立端口**：短信发送流速达800条/秒。


### 应用场景

-   **注册登录**

    短信验证码直接登录和注册，无需输入密码，简化流程，提升注册转化率。

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/f446577839ff40d694e970aa4c4120db~tplv-k3u1fbpfcp-zoom-1.image)

-   **找回密码**

      用户用短信验证码进行密码找回，免除复杂的安全问题以及认证环节，安全快速。

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/134b7a1ac7ec4aa68cc3a0e7c0210e15~tplv-k3u1fbpfcp-zoom-1.image)

-   **支付认证**

    重要账户、大额支付短信验证，做好安全风控，为您的资金财产保驾护航。

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/1c4d0ad6709640c4839914af594a2d1a~tplv-k3u1fbpfcp-zoom-1.image)

-   **更改信息**

    用户更改注册管理重要信息的时候，通过填入手机验证码，一键操作，安全提供便捷。

![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/cb32544ec918437e997e47d4b2233381~tplv-k3u1fbpfcp-zoom-1.image)


### 签名规范

| 类别   | 规范说明                                                                                                                                                                                                                                                                                                                                                                  |
| ---- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 签名内容 | 1、建议签名内容为短信发送方的真实应用名称。 2、短信签名作为短信发送者属性的一种标识，签名必须用于标识产品名称或业务，禁止发送涉及：色情、赌博、毒品、党政、法律维权、众筹、慈善募捐、宗教、迷信、股票、留学移民、面试招聘、博彩、贷款、催款还款、信用卡提额、投资理财、中奖、抽奖、一元夺宝、一元秒杀、一元云购、二类电商、A货、烟酒、交友、暴力、恐吓、皮草、返现返利、代开发票、运营商禁止发送的信息、代理注册、代办证件、加群、加QQ或者加微信、贩卖个人信息、运营商业务、流量营销、违反广告法用语、殡葬、刷单、做任务、空包网、邀请好评、转店类、拉新、众包业务等内容的短信。 若签名内容侵犯到第三方权益，必须获得第三方授权。 3、短信签名必须具有实际意义。不支持含义模糊的中性签名，如“测试”、“客服通知”、“客户您好”等 |
| 签名审核 | 签名将由人工审核后方可启用，填写的应用场景可视情况填写，至少填写一个，越详细真实的应用场景，审核通过概率越高                                                                                                                                                                                                                                                                                                                |
| 长度   | 字数要求2-20个字符                                                                                                                                                                                                                                                                                                                                                           |
| 格式   | 公司或品牌名称，不能使用空格和特殊符号"- + * & % # @ ~"等，运营商规定发送短信必须带签名                                                                                                                                                                                                                                                                                                                |

  


### 模板规范

| 类别   | 规范说明                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 模板内容 | 短信模板需明确表述短信发送的实际内容。所有模板均禁止发送金融相关的所有内容。不支持发送未经许可的信息，主要指邀请注册、邀请成为会员的商业性信息。禁止发送涉及：色情、赌博、毒品、党政、法律维权、众筹、慈善募捐、宗教、迷信、股票、留学移民、面试招聘、博彩、贷款、催款还款、信用卡提额、投资理财、中奖、抽奖、一元夺宝、一元秒杀、一元云购、二类电商、A货、烟酒、交友、暴力、恐吓、皮草、返现返利、代开发票、运营商禁止发送的信息、代理注册、代办证件、加群、加QQ或者加微信、贩卖个人信息、运营商业务、流量营销、违反广告法用语、殡葬、刷单、做任务、空包网、邀请好评、转店类、拉新、众包业务、POS机、积分兑换等内容的短信。禁止在关键字或关键信息中出现错别字、变体字、异体字、各类干扰符号等；禁止出现各类非正常混合字以及非常用的表达法。不支持内容中含有直接或间接访问应用内测分发平台的行为。地产、留学、招聘、交友、游戏等行业仅支持发送验证码短信。 |
| 模板审核 | ●签名跟模板报备的情况下，短信发送将直接提交给网关。 ●如果出现批量短信发送驳回的情况，可能为“敏感词拦截”进入人工审核，请联系客服。                                                                                                                                                                                                                                                                                                                                                              |
| 格式   | ●内容首尾不能添加【】。 ●链接地址请写在短信内容中，便于核实，部分安卓系统存在链接识别问题，需在链接前后添加空格。                                                                                                                                                                                                                                                                                                                                                                       |
| 计费   | ●短信字数 <=70个字，按照70个字一条短信计算。中文英文符号统一计算为一个字符。 ●短信字数>70个字，占用3个字符作为分条字符，按照67个字记为一条短信计算，多条短信可能在部分手机系统上呈现为一条短信的形态，测试时请注意。                                                                                                                                                                                                                                                                                                               |

### 模板示例

1.  【Eolink】您的注册验证码是{$var}，有效时间5分钟。如非本人操作，请忽略本短信。
1.  【Eolink】您正在找回密码，您的验证码是{$var}。如非本人操作，请忽略本短信。
1.  【Eolink】您正在修改密码，您的验证码是{$var}。如非本人操作，请忽略本短信。
1.  【Eolink】您正在登录，您的验证码是{$var}。如非本人操作，请忽略本短信。
1.  【Eolink】您正在进行身份认证，您的验证码是{$var}。如非本人操作，请忽略本短信。
1.  【Eolink】您正在绑定手机，您的验证码是{$var}。如非本人操作，请忽略本短信。

### Python(Requests) 调用代码示例

```
import requests

url = "https://eolink.o.apispace.com/sms-code/verifycode"

payload = {"msg":"【Eolinker】您的验证码是：{$var}，5分钟内有效。如非本人操作，请忽略。","params":"15800000000,1234;13800000000,4321","sendtime":"","extend":"","uid":""}

headers = {
    "X-APISpace-Token":"",
    "Authorization-Type":"apikey",
    "Content-Type":"application/json"
}

response=requests.request("POST", url, data=json.dumps(payload), headers=headers)

print(response.text)

```
