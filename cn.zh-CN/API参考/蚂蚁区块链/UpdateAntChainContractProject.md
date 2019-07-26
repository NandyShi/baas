# UpdateAntChainContractProject {#doc_api_Baas_UpdateAntChainContractProject .reference}

在联盟内更新一个合约工程的属性

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=UpdateAntChainContractProject&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ProjectId|String|是|bDXK1b8Z|合约工程ID

 |
|Action|String|否|UpdateAntChainContractProject|系统规定参数。取值：UpdateAntChainContractProject。

 |
|ProjectDescription|String|否|合约工程的版本描述|合约工程描述

 |
|ProjectName|String|否|更新合约工程名称|合约工程名称

 |
|ProjectVersion|String|否|v1.1.1|合约工程版本

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|9EBD381E-A19E-4875-8771-EDA08A0416D3|请求ID

 |
|Result|String|success|请求结果

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=UpdateAntChainContractProject
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"9EBD381E-A19E-4875-8771-EDA08A0416D3",
	"data":{
		"Result":"success",
		"RequestId":"9EBD381E-A19E-4875-8771-EDA08A0416D3"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

