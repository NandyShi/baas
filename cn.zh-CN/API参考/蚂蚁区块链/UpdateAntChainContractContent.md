# UpdateAntChainContractContent {#doc_api_Baas_UpdateAntChainContractContent .reference}

更新一个合约工程的内容

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=UpdateAntChainContractContent&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ContentId|String|是|R6XMn59e|文件ID

 |
|ParentContentId|String|是|R38DYDop|上级目录ID

 |
|Action|String|否|UpdateAntChainContractContent|系统规定参数。取值：UpdateAntChainContractContent。

 |
|Content|String|否|update content|文件内容

 |
|ContentName|String|否|newFile|更新文件/文件夹名称

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|08CBD579-C430-4F1F-9011-C120FA1E9B97|请求ID

 |
|Result|String|success|请求结果

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=UpdateAntChainContractContent
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"08CBD579-C430-4F1F-9011-C120FA1E9B97",
	"data":{
		"Result":"success",
		"RequestId":"08CBD579-C430-4F1F-9011-C120FA1E9B97"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

