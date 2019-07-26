# DescribeAntChainInformation {#doc_api_Baas_DescribeAntChainInformation .reference}

查询一条蚂蚁区块链的基本信息

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainInformation&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|pYogqb9v|区块链ID

 |
|Action|String|否|DescribeAntChainInformation|系统规定参数。取值：DescribeAntChainInformation。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|91246411-C7E9-4EFD-9074-3939AEDFC1BB|请求ID

 |
|Result| | |请求结果

 |
|AbnormalNodes|Integer|0|异常节点数

 |
|AntChainId|String|pYogqb9v|区块链ID

 |
|BlockHeight|Integer|365236|区块链高度

 |
|CreateTime|Long|1562847396000|创建时戳

 |
|NodeInfos| | |节点信息

 |
|BlockHeight|Long|365216|区块链高度

 |
|NodeName|String|121.199.195.8 18130|节点地址

 |
|Status|Boolean|true|节点状态

 |
|Version|String|0.10|运行版本

 |
|NodeNumber|Integer|4|节点总数

 |
|Normal|Boolean|true|运行状态

 |
|TransactionSum|Integer|42|交易总数

 |
|Version|String|0.10.2.4.7|区块链版本

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainInformation
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"91246411-C7E9-4EFD-9074-3939AEDFC1BB",
	"data":{
		"Result":{
			"NodeNumber":4,
			"AbnormalNodes":0,
			"BlockHeight":365236,
			"IsRole":false,
			"Normal":true,
			"TransactionSum":42,
			"CreateTime":1562847396000,
			"AntChainId":"pYogqb9v",
			"Version":"0.10.2.4.7",
			"NodeInfos":[
				{
					"Status":true,
					"BlockHeight":365216,
					"Version":"0.10",
					"NodeName":"121.199.195.8 18130"
				},
				{
					"Status":true,
					"BlockHeight":365216,
					"Version":"0.10",
					"NodeName":"121.199.195.8 18132"
				},
				{
					"Status":true,
					"BlockHeight":365216,
					"Version":"0.10",
					"NodeName":"121.199.195.8 18133"
				},
				{
					"Status":true,
					"BlockHeight":365216,
					"Version":"0.10",
					"NodeName":"121.199.195.8 18131"
				}
			]
		},
		"RequestId":"91246411-C7E9-4EFD-9074-3939AEDFC1BB"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

