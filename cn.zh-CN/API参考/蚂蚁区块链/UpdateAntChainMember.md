# UpdateAntChainMember {#doc_api_Baas_UpdateAntChainMember .reference}

更新联盟成员属性

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=UpdateAntChainMember&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|UpdateAntChainMember|系统规定参数。取值：UpdateAntChainMember。

 |
|ConsortiumId|String|是|AroN3X2l|联盟ID

 |
|MemberId|String|是|1287126353301234|成员ID

 |
|MemberName|String|是|updatename|成员名称

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|5BA242B2-AB0C-4D06-94EB-23CEC4F7B95E|请求ID

 |
|Result|String|success|请求结果

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=UpdateAntChainMember
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<xml version="1.0" encoding="UTF-8">
	  <code>200</code>
	  <data>
		    <RequestId>5BA242B2-AB0C-4D06-94EB-23CEC4F7B95E</RequestId>
		    <Result>success</Result>
	  </data>
	  <requestId>5BA242B2-AB0C-4D06-94EB-23CEC4F7B95E</requestId>
	  <successResponse>true</successResponse>
</xml>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"5BA242B2-AB0C-4D06-94EB-23CEC4F7B95E",
	"data":{
		"Result":"success",
		"RequestId":"5BA242B2-AB0C-4D06-94EB-23CEC4F7B95E"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

