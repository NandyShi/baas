# DescribeFabricInviter {#doc_api_Baas_DescribeFabricInviter .reference}

调用DescribeFabricInviter获取邀请人信息。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricInviter&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Code|String|是|200|邀请码

 |
|Action|String|否|DescribeFabricInviter|系统规定参数。取值：**DescribeFabricInviter**。

 |
|RegionId|String|否|cn-hangzhou|地域

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|ErrorCode|Integer|200|错误码

 |
|RequestId|String|C445762C-8909-4BD8-A2BD-BB45BF2441D8|请求ID

 |
|Result| | |邀请人信息列表

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwl\*\*\*\*|联盟ID

 |
|ConsortiumName|String|name|联盟名称

 |
|ExpireTime|String|1544411108000|过期时间

 |
|InviterId|Long|3524234|邀请者ID

 |
|InviterName|String|name|邀请者

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricInviter
&Code=200
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricInviterResponse>
	  <Result>
		    <ConsortiumId>10000</ConsortiumId>
		    <ExpireTime>1544411108000</ExpireTime>
		    <InviterId>35242340</InviterId>
		    <ConsortiumName>quickstart</ConsortiumName>
		    <InviterName>name</InviterName>
	  </Result>
	  <RequestId>C445762C-8909-4BD8-A2BD-BB45BF2441D8</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricInviterResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"ConsortiumName":"quickstart",
			"ConsortiumId":"10000",
			"InviterName":"name",
			"ExpireTime":1544411108000,
			"InviterId":35242340
		}
	],
	"RequestId":"C445762C-8909-4BD8-A2BD-BB45BF2441D8",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

