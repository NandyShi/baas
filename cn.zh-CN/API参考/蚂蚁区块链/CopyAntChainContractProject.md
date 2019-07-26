# CopyAntChainContractProject {#doc_api_Baas_CopyAntChainContractProject .reference}

在联盟内复制一个已有的合约工程

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CopyAntChainContractProject&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ProjectId|String|是|2L9VK68g|工程ID

 |
|ProjectName|String|是|copyproject|工程名

 |
|ProjectVersion|String|是|v1.0.1|工程版本

 |
|Action|String|否|CopyAntChainContractProject|系统规定参数。取值：CopyAntChainContractProject。

 |
|ProjectDescription|String|否|copy project description|工程描述

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|45D67F6F-C723-4AD8-8462-F94EE5FF22E6|请求ID

 |
|Result| | |请求结果

 |
|ConsortiumId|String|DV80nJXq|联盟ID

 |
|CreateTime|Long|1563953475248|创建时间

 |
|ProjectDescription|String|copy project description|工程描述

 |
|ProjectId|String|R6XMEdXe|工程ID

 |
|ProjectName|String|copyproject|工程名称

 |
|ProjectVersion|String|v1.0.1|工程版本

 |
|UpdateTime|Long|1563953475248|更新时间

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CopyAntChainContractProject
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"45D67F6F-C723-4AD8-8462-F94EE5FF22E6",
	"data":{
		"Result":{
			"ProjectDescription":"copy project description",
			"ProjectName":"copyproject",
			"ConsortiumId":"DV80nJXq",
			"ProjectVersion":"v1.0.1",
			"CreateTime":1563953475248,
			"UpdateTime":1563953475248,
			"ProjectId":"R6XMEdXe"
		},
		"RequestId":"45D67F6F-C723-4AD8-8462-F94EE5FF22E6"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

