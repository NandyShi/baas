# DescribeAntChainBlock {#doc_api_Baas_DescribeAntChainBlock .reference}

根据块高查询一条蚂蚁区块链的区块信息

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainBlock&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|pYogqb9v|区块链ID

 |
|Height|Long|是|1234|查询区块高度

 |
|Action|String|否|DescribeAntChainBlock|系统规定参数。取值：DescribeAntChainBlock。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|4DDA2E72-778A-4D79-BE70-448A26A57227|请求ID

 |
|Result| | |请求结果

 |
|AntChainId|String|pYogqb9v|区块链ID

 |
|BlockHash|String|aeec5963f8deeeae820aaf302f0c925db9fa8d07b9898dac782335f817554e47|区块哈希

 |
|CreateTime|Long|1562851727742|创建时间

 |
|Height|Integer|1234|区块高度

 |
|PreviousHash|String|e11767c7b9d92563663a76f10c69e8354788001e2c9e6bd9267239a81d3bb523|前一个区块链哈希

 |
|RootTxHash|String|0000000000000000000000000000000000000000000000000000000000000000|根交易哈希

 |
|TransSummaryList|String|\[\]|交易列表

 |
|TransactionSize|Integer|0|交易数

 |
|Version|Long|2|区块版本

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainBlock
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"4DDA2E72-778A-4D79-BE70-448A26A57227",
	"data":{
		"Result":{
			"PreviousHash":"e11767c7b9d92563663a76f10c69e8354788001e2c9e6bd9267239a81d3bb523",
			"BlockHash":"aeec5963f8deeeae820aaf302f0c925db9fa8d07b9898dac782335f817554e47",
			"RootTxHash":"0000000000000000000000000000000000000000000000000000000000000000",
			"TransSummaryList":[],
			"CreateTime":1562851727742,
			"Height":1234,
			"AntChainId":"pYogqb9v",
			"TransactionSize":0,
			"Version":2
		},
		"RequestId":"4DDA2E72-778A-4D79-BE70-448A26A57227"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

