# DescribeFabricInvitationCode {#doc_api_Baas_DescribeFabricInvitationCode .reference}

调用DescribeFabricInvitationCode获取邀请链接。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricInvitationCode&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricInvitationCode|系统规定参数。取值：**DescribeFabricInvitationCode**。

 |
|ConsortiumId|String|是|consortium-lianmenyumingyi-hc5d1bwl\*\*\*\*|联盟ID

 |
|RegionId|String|否|cn-hangzhou|地域

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|DynamicCode|String|InvitationCodeNotFound|错误代码

 |
|DynamicMessage|String|The invitation code could not found.|错误消息

 |
|ErrorCode|Integer|200|错误码

 |
|RequestId|String|77E25463-56CB-4F1C-8EB6-8ADDFE39EF0F|请求ID

 |
|Result| | |邀请链接列表

 |
|Accepted|Boolean|true|是否接受

 |
|Code|String|code|邀请码

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

 |
|Email|String|abc@126.com|邮箱

 |
|ExpireTime|String|1544411108000|过期时间

 |
|InvitationId|Integer|2|邀请ID

 |
|SendTime|String|1544411108000|发送时间

 |
|SenderBid|String|27534|发送者Bid

 |
|SenderId|Long|26345345|发送者ID

 |
|SenderName|String|uid-35324|发送者

 |
|Url|String|http://baas.console.aliyun.test/invite?code=92e7ef1934892|邀请链接

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricInvitationCode
&ConsortiumId=consortium-lianmenyumingyi-hc5d1bwl****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricInvitationCodeResponse>
  <Result>
		    <Url>http://baas.console.aliyun.test/invite?code=92e7ef1934892f272537d750c743a3d1be773038c97a8414065d63551a742b81</Url>
		    <ExpireTime>2018-06-14T15:10:11.000+0000</ExpireTime>
		    <Accepted>true</Accepted>
		    <Code>code</Code>
		    <ConsortiumId>consortium-lianmenyumingyi-hc5d1bwlulg7</ConsortiumId>
		    <Email>abc@126.com</Email>
		    <InvitationId>2</InvitationId>
		    <SendTime>2018-06-14T15:10:11.000+0000</SendTime>
		    <SenderId>126467457</SenderId>
		    <SenderBid>3563</SenderBid>
		    <SenderName>name</SenderName>
	  </Result>
	  <RequestId>9CFDE6E9-3835-4C2E-BECD-7CF20F5B5DD7</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricInvitationCodeResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"SenderBid":"3563",
		"Email":"abc@126.com",
		"ConsortiumId":"consortium-lianmenyumingyi-hc5d1bwlulg7",
		"Url":"http://baas.console.aliyun.test/invite?code=92e7ef1934892f272537d750c743a3d1be773038c97a8414065d63551a742b81",
		"InvitationId":2,
		"Accepted":"true",
		"ExpireTime":"2018-06-14T15:10:11.000+0000",
		"SendTime":"2018-06-14T15:10:11.000+0000",
		"SenderId":126467457,
		"SenderName":"name",
		"Code":"code"
	},
	"RequestId":"9CFDE6E9-3835-4C2E-BECD-7CF20F5B5DD7",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

