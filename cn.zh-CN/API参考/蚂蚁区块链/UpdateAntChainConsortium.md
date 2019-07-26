# UpdateAntChainConsortium {#doc_api_Baas_UpdateAntChainConsortium .reference}

更新联盟属性

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=UpdateAntChainConsortium&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ConsortiumDescription|String|是|测试联盟|联盟描述

 |
|ConsortiumId|String|是|q0oWq92P|联盟ID

 |
|ConsortiumName|String|是|联盟名称|联盟名称

 |
|Action|String|否|UpdateAntChainConsortium|系统规定参数。取值：UpdateAntChainConsortium。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|1E55C947-19B4-4AAD-9D22-0B8DA8904B3D|请求ID

 |
|Result|String|success|请求结果

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=UpdateAntChainConsortium
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<xml version="1.0" encoding="UTF-8">
	  <code>200</code>
	  <data>
		    <RequestId>1E55C947-19B4-4AAD-9D22-0B8DA8904B3D</RequestId>
		    <Result>success</Result>
	  </data>
	  <requestId>1E55C947-19B4-4AAD-9D22-0B8DA8904B3D</requestId>
	  <successResponse>true</successResponse>
</xml>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"1E55C947-19B4-4AAD-9D22-0B8DA8904B3D",
	"data":{
		"Result":"success",
		"RequestId":"1E55C947-19B4-4AAD-9D22-0B8DA8904B3D"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

