# ResetAntChainUserCertificate {#doc_api_Baas_ResetAntChainUserCertificate .reference}

重置用户

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=ResetAntChainUserCertificate&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|bDXK6boZ|区块链ID

 |
|Bid|String|是|26842|Bid

 |
|Operation|Integer|是|1|操作类型

 |
|Username|String|是|uid-1287126353308684|用户名

 |
|Action|String|否|ResetAntChainUserCertificate|系统规定参数。取值：ResetAntChainUserCertificate。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|3EB828D1-1E9D-4EC2-A002-139FE998D674|请求ID

 |
|Result|String|success|请求结果

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=ResetAntChainUserCertificate
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"3EB828D1-1E9D-4EC2-A002-139FE998D674",
	"data":{
		"Result":"success",
		"RequestId":"3EB828D1-1E9D-4EC2-A002-139FE998D674"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

