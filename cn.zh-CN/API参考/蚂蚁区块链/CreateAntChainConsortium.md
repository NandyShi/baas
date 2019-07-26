# CreateAntChainConsortium {#doc_api_Baas_CreateAntChainConsortium .reference}

创建联盟

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CreateAntChainConsortium&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ConsortiumName|String|是|联盟名称|联盟名称

 |
|Action|String|否|CreateAntChainConsortium|系统规定参数。取值：CreateAntChainConsortium。

 |
|ConsortiumDescription|String|否|联盟描述|联盟描述

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|87FAFC6B-E7AE-4626-B7F7-AE0B88E612D5|请求ID

 |
|Result| | |请求结果

 |
|ConsortiumId|String|A28nO1ow|联盟ID

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CreateAntChainConsortium
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"87FAFC6B-E7AE-4626-B7F7-AE0B88E612D5",
	"data":{
		"Result":{
			"ConsortiumId":"A28nO1ow"
		},
		"RequestId":"87FAFC6B-E7AE-4626-B7F7-AE0B88E612D5"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

