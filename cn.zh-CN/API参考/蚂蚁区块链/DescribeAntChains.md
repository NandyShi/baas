# DescribeAntChains {#doc_api_Baas_DescribeAntChains .reference}

获取联盟内的蚂蚁区块链列表

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChains&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ConsortiumId|String|是|AroN3X2l|联盟ID

 |
|PageNumber|Integer|是|1|当前页面编号

 |
|PageSize|Integer|是|20|页面条例数

 |
|Action|String|否|DescribeAntChains|系统规定参数。取值：DescribeAntChains。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|52EC3196-D0B8-4FBE-A8B6-6DDABABE11C9|请求ID

 |
|Result| | |请求结果

 |
|AntChains| | |蚂蚁区块链属性描述

 |
|AntChainId|String|pYogqb9v|蚂蚁区块链ID

 |
|AntChainName|String|一个测试的区块链|区块链名称

 |
|ChainType|String|Contract|区块链类型

 |
|CipherSuit|String|classic|加密套件类型

 |
|CreateTime|Long|1562847396000|创建时戳

 |
|ExpireTime|Long|1626019200000|到期时间

 |
|IsAdmin|Boolean|true|当前用户是否是管理员

 |
|MemberStatus|String|ChainApplied|是否已经申请链上访问证书

 |
|MerkleTreeSuit|String|fdmt|Merkle树类型

 |
|Network|String|Running|运行状态

 |
|NodeNum|Integer|4|节点数量

 |
|RegionId|String|cn-hangzhou|创建地域信息

 |
|ResourceSize|String|Basic|区块链类型

 |
|TlsAlgo|String|rsa|TLS加密算法

 |
|IsExist|Boolean|false|是否存在

 |
|Pagination| | |分页情况

 |
|PageNumber|Integer|1|当前页面编号

 |
|PageSize|Integer|20|每页显示条例数

 |
|TotalCount|Integer|1|总数

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChains
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"06EA0FF7-6D9E-41A6-8652-6536F1C5304F",
	"data":{
		"Result":{
			"AntChains":[
				{
					"TlsAlgo":"rsa",
					"CipherSuit":"classic",
					"MerkleTreeSuit":"fdmt",
					"IsAdmin":true,
					"MemberStatus":"ChainApplied",
					"NodeNum":4,
					"AntChainName":"一个测试的区块链",
					"ResourceSize":"Basic",
					"Network":"Running",
					"ExpireTime":1626019200000,
					"CreateTime":1562847396000,
					"RegionId":"cn-hangzhou",
					"ChainType":"Contract",
					"AntChainId":"pYogqb9v"
				}
			],
			"Pagination":{
				"PageNumber":1,
				"TotalCount":1,
				"PageSize":20
			},
			"IsExist":false
		},
		"RequestId":"06EA0FF7-6D9E-41A6-8652-6536F1C5304F"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

