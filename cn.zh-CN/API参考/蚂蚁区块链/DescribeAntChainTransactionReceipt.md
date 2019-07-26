# DescribeAntChainTransactionReceipt {#doc_api_Baas_DescribeAntChainTransactionReceipt .reference}

根据交易哈希查询一条蚂蚁区块链的交易回执信息

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainTransactionReceipt&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|pYogqb9v|区块链ID

 |
|Hash|String|是|b3b0d2db83d3e670449d1e2a39d1d13b7e0e6080b0f9c6945f79eca68d1dd2ca|交易哈希

 |
|Action|String|否|DescribeAntChainTransactionReceipt|系统规定参数。取值：DescribeAntChainTransactionReceipt。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|9EC8FDC1-ED32-4EC0-AEC2-AFAA906ADBAB|请求ID

 |
|Result| | |请求结果

 |
|Data|String|data|Data

 |
|GasUsed|String|20000|消耗的Gas

 |
|Logs| |\[""\]|logs

 |
|Result|Long|0|结果

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainTransactionReceipt
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"9EC8FDC1-ED32-4EC0-AEC2-AFAA906ADBAB",
	"data":{
		"Result":{
			"Result":0,
			"Logs":[
				""
			],
			"Data":"",
			"GasUsed":"20000"
		},
		"RequestId":"9EC8FDC1-ED32-4EC0-AEC2-AFAA906ADBAB"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

