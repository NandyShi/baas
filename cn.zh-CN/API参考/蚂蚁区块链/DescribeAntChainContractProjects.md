# DescribeAntChainContractProjects {#doc_api_Baas_DescribeAntChainContractProjects .reference}

获取联盟内合约工程的列表

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainContractProjects&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ConsortiumId|String|是|DV80nJXq|联盟ID

 |
|PageNumber|Integer|是|1|页面编号

 |
|PageSize|Integer|是|10|每页数量

 |
|Action|String|否|DescribeAntChainContractProjects|系统规定参数。取值：DescribeAntChainContractProjects。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|5EDAC16F-EA3E-4017-B223-D76220F985DF|请求ID

 |
|Result| | |请求结果

 |
|ContractProjects| | |合约工程

 |
|ConsortiumId|String|DV80nJXq|联盟ID

 |
|CreateTime|Long|1562847564000|创建时间

 |
|ProjectDescription|String|description|工程描述

 |
|ProjectId|String|2L9VK68g|工程ID

 |
|ProjectName|String|projectname|工程名称

 |
|ProjectVersion|String|5|工程版本

 |
|UpdateTime|Long|1563954499000|更新时间

 |
|Pagination| | |分页信息

 |
|PageNumber|Integer|1|页面编号

 |
|PageSize|Integer|10|每页数量

 |
|TotalCount|Integer|1|总数

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainContractProjects
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"5EDAC16F-EA3E-4017-B223-D76220F985DF",
	"data":{
		"Result":{
			"Pagination":{
				"PageNumber":1,
				"TotalCount":1,
				"PageSize":10
			},
			"ContractProjects":[
				{
					"ProjectDescription":"",
					"ProjectName":"projectname",
					"ConsortiumId":"DV80nJXq",
					"ProjectVersion":"5",
					"CreateTime":1562847564000,
					"UpdateTime":1563954499000,
					"ProjectId":"2L9VK68g"
				}
			]
		},
		"RequestId":"5EDAC16F-EA3E-4017-B223-D76220F985DF"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

