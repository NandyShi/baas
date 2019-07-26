# DeleteAntChainContractContent {#doc_api_Baas_DeleteAntChainContractContent .reference}

删除一个合约工程的内容

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DeleteAntChainContractContent&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ContentId|String|是|GKX7KZX0|文件ID

 |
|Action|String|否|DeleteAntChainContractContent|系统规定参数。取值：DeleteAntChainContractContent。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|7E54F588-39DE-446F-9A16-B9BB0B05DF44|请求ID

 |
|Result|String|success|请求结果

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DeleteAntChainContractContent
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"7E54F588-39DE-446F-9A16-B9BB0B05DF44",
	"data":{
		"Result":"success",
		"RequestId":"7E54F588-39DE-446F-9A16-B9BB0B05DF44"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

