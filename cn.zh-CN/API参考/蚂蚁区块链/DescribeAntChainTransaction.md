# DescribeAntChainTransaction {#doc_api_Baas_DescribeAntChainTransaction .reference}

根据交易哈希查询一条蚂蚁区块链的交易信息

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainTransaction&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|pYogqb9v|区块链ID

 |
|Hash|String|是|b3b0d2db83d3e670449d1e2a39d1d13b7e0e6080b0f9c6945f79eca68d1dd2ca|交易哈希

 |
|Action|String|否|DescribeAntChainTransaction|系统规定参数。取值：DescribeAntChainTransaction。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|7DCE6520-E5DB-4859-90AC-BDDB8A5501C6|请求ID

 |
|Result| | |请求结果

 |
|BlockHash|String|1168bc5dd0b78d15446b15ea5a7f7822a7d07c007dd3a50becf98da220fc08f6|区块哈希

 |
|BlockHeight|Long|368169|区块高度

 |
|BlockVersion|String|10|区块版本

 |
|CreateTime|Long|1563954336850|交易创建时间

 |
|Hash|String|b3b0d2db83d3e670449d1e2a39d1d13b7e0e6080b0f9c6945f79eca68d1dd2ca|交易哈希

 |
|Transaction| | |交易详情

 |
|Data|String|“”|数据

 |
|Extentions| |\[\]|扩展信息

 |
|From|String|e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b|交易发送者哈希

 |
|Gas|String|4000000|Gas值

 |
|Hash|String|b3b0d2db83d3e670449d1e2a39d1d13b7e0e6080b0f9c6945f79eca68d1dd2ca|交易哈希

 |
|Nonce|String|5675407026657953619|交易Nonce

 |
|Period|Long|1563954336850|Period

 |
|Signatures| |5s6JhauIqAlMb6d+7...|签名

 |
|Timestamp|Long|1563954336850|交易发送时戳

 |
|To|String|961085f3c7ef705ad587d0cbe11d7863a5a11af7451f4e9b1edadd74402addf5|交易接收方地址

 |
|TxType|String|UNFREEZE\_ACCOUNT\_CONTRACT|交易类型

 |
|Value|String|0|交易金额

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainTransaction
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"7DCE6520-E5DB-4859-90AC-BDDB8A5501C6",
	"data":{
		"Result":{
			"Hash":"b3b0d2db83d3e670449d1e2a39d1d13b7e0e6080b0f9c6945f79eca68d1dd2ca",
			"BlockHeight":368169,
			"Transaction":{
				"Period":1563954336850,
				"Hash":"b3b0d2db83d3e670449d1e2a39d1d13b7e0e6080b0f9c6945f79eca68d1dd2ca",
				"Value":"0",
				"To":"961085f3c7ef705ad587d0cbe11d7863a5a11af7451f4e9b1edadd74402addf5",
				"Extentions":[],
				"Signatures":[
					"5s6JhauIqAlMb6d+7..."
				],
				"TxType":"UNFREEZE_ACCOUNT_CONTRACT",
				"Nonce":"5675407026657953619",
				"Timestamp":1563954336850,
				"From":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"Gas":"4000000"
			},
			"CreateTime":1563954336850,
			"BlockVersion":10
		},
		"RequestId":"7DCE6520-E5DB-4859-90AC-BDDB8A5501C6"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

