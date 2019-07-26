# CreateAntChainContractContent {#doc_api_Baas_CreateAntChainContractContent .reference}

创建一个合约工程的内容，可以是文件或者文件夹

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CreateAntChainContractContent&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ContentName|String|是|newFile|新建文件/文件夹内容

 |
|IsDirectory|Boolean|是|false|是否是文件夹

 |
|ParentContentId|String|是|R38DYDop|上级目录ID

 |
|ProjectId|String|是|bDXK1b8Z|合约工程ID

 |
|Action|String|否|CreateAntChainContractContent|系统规定参数。取值：CreateAntChainContractContent。

 |
|Content|String|否|""|新建文件/文件夹内容

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|C407F102-062A-44B3-BBDC-E3B2718F633D|请求ID

 |
|Result| | |请求结果

 |
|Content|String|""|新建文件/文件夹内容

 |
|ContentId|String|R6XMn59e|新建文件/文件夹ID

 |
|ContentName|String|newFile|新建文件/文件夹名称

 |
|CreateTime|String|1564024964404|创建时间

 |
|IsDirectory|Boolean|false|是否是目录

 |
|ParentContentId|String|R38DYDop|上级目录ID

 |
|ProjectId|String|bDXK1b8Z|合约工程ID

 |
|UpdateTime|String|1564024964404|更新时间

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CreateAntChainContractContent
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"C407F102-062A-44B3-BBDC-E3B2718F633D",
	"data":{
		"Result":{
			"ParentContentId":"R38DYDop",
			"IsDirectory":false,
			"CreateTime":1564024964404,
			"ContentId":"R6XMn59e",
			"UpdateTime":1564024964404,
			"ContentName":"newFile",
			"Content":"",
			"ProjectId":"bDXK1b8Z"
		},
		"RequestId":"C407F102-062A-44B3-BBDC-E3B2718F633D"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

