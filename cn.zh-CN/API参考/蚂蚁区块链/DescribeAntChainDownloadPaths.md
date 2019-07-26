# DescribeAntChainDownloadPaths {#doc_api_Baas_DescribeAntChainDownloadPaths .reference}

获取一条蚂蚁区块链相关证书下载地址

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainDownloadPaths&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|1q8B5R9p|区块链ID

 |
|Action|String|否|DescribeAntChainDownloadPaths|系统规定参数。取值：DescribeAntChainDownloadPaths。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|E6F487D4-8606-41B5-B289-46D5EFBD3417|请求ID

 |
|Result| | |请求结果

 |
|CaCrtUrl|String|http://\*\*\*ca.crt|ca.crt下载链接

 |
|ClientCrtUrl|String|http://\*\*\*client.crt|client.crt下载链接

 |
|SdkUrl|String|http://\*\*\*|sdk下载链接

 |
|TrustCaUrl|String|http://\*\*\*trustCa|trustCA下载链接

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainDownloadPaths
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"E6F487D4-8606-41B5-B289-46D5EFBD3417",
	"data":{
		"Result":{
			"SdkUrl":"http://***",
			"TrustCaUrl":"http://***trustCa",
			"CaCrtUrl":"http://***a.crt",
			"ClientCrtUrl":"http://***client.crt"
		},
		"RequestId":"E6F487D4-8606-41B5-B289-46D5EFBD3417"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

