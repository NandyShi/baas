# DescribeAntChainTransactionStatistics {#doc_api_Baas_DescribeAntChainTransactionStatistics .reference}

查询一条蚂蚁区块链的交易统计信息

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainTransactionStatistics&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|pYogqb9v|区块链ID

 |
|Action|String|否|DescribeAntChainTransactionStatistics|系统规定参数。取值：DescribeAntChainTransactionStatistics。

 |
|End|Long|否|1563897600000|统计结束时间

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |
|Start|Long|否|1563206400000|统计开始时间

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|E93884AC-6C21-4FEA-8E3A-7377D33B194F|请求ID

 |
|Result| | |请求结果

 |
|AntChainId|String|pYogqb9v|区块链ID

 |
|CreatTime|Long|1563294007000|创建时间

 |
|Dt|String|2019-07-16|时间

 |
|LastSumBlockHeight|Long|148018|最后统计的区块高度

 |
|TransCount|Long|0|交易总量

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainTransactionStatistics
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"E93884AC-6C21-4FEA-8E3A-7377D33B194F",
	"data":{
		"Result":[
			{
				"TransCount":0,
				"Dt":"2019-07-16",
				"AntChainId":"pYogqb9v",
				"LastSumBlockHeight":148018,
				"CreatTime":1563294007000
			},
			{
				"TransCount":1,
				"Dt":"2019-07-17",
				"AntChainId":"pYogqb9v",
				"LastSumBlockHeight":176768,
				"CreatTime":1563380401000
			},
			{
				"TransCount":0,
				"Dt":"2019-07-18",
				"AntChainId":"pYogqb9v",
				"LastSumBlockHeight":205517,
				"CreatTime":1563466809000
			},
			{
				"TransCount":0,
				"Dt":"2019-07-19",
				"AntChainId":"pYogqb9v",
				"LastSumBlockHeight":234268,
				"CreatTime":1563553209000
			},
			{
				"TransCount":0,
				"Dt":"2019-07-20",
				"AntChainId":"pYogqb9v",
				"LastSumBlockHeight":263020,
				"CreatTime":1563639601000
			},
			{
				"TransCount":0,
				"Dt":"2019-07-21",
				"AntChainId":"pYogqb9v",
				"LastSumBlockHeight":291772,
				"CreatTime":1563726001000
			},
			{
				"TransCount":1,
				"Dt":"2019-07-22",
				"AntChainId":"pYogqb9v",
				"LastSumBlockHeight":320523,
				"CreatTime":1563812401000
			},
			{
				"TransCount":26,
				"Dt":"2019-07-23",
				"AntChainId":"pYogqb9v",
				"LastSumBlockHeight":349284,
				"CreatTime":1563898810000
			}
		],
		"RequestId":"E93884AC-6C21-4FEA-8E3A-7377D33B194F"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

