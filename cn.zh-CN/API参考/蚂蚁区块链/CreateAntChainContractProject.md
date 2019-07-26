# CreateAntChainContractProject {#doc_api_Baas_CreateAntChainContractProject .reference}

在联盟内创建一个合约工程

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CreateAntChainContractProject&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ConsortiumId|String|是|DV80nJXq|联盟ID

 |
|ProjectName|String|是|projectname|项目名称

 |
|ProjectVersion|String|是|v1.0.0|项目版本

 |
|Action|String|否|CreateAntChainContractProject|系统规定参数。取值：CreateAntChainContractProject。

 |
|ProjectDescription|String|否|project description|工程描述

 |
|RegionId|String|否|cn-hangzhou|区域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|4261A4C3-B8B5-4555-AEBC-944C3EAB23DB|请求ID

 |
|Result| | |请求结果

 |
|ConsortiumId|String|DV80nJXq|联盟ID

 |
|CreateTime|Long|1563951889044|创建时间

 |
|ProjectDescription|String|project description|工程描述

 |
|ProjectId|String|R38DAbop|工程ID

 |
|ProjectName|String|projectname|工程名称

 |
|ProjectVersion|String|v1.0.0|工程版本

 |
|UpdateTime|Long|1563951889140|更新时间

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CreateAntChainContractProject
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"4261A4C3-B8B5-4555-AEBC-944C3EAB23DB",
	"data":{
		"Result":{
			"ProjectDescription":"project description",
			"ProjectName":"projectname",
			"ConsortiumId":"DV80nJXq",
			"ProjectVersion":"v1.0.0",
			"CreateTime":1563951889044,
			"UpdateTime":1563951889140,
			"ProjectId":"R38DAbop"
		},
		"RequestId":"4261A4C3-B8B5-4555-AEBC-944C3EAB23DB"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

