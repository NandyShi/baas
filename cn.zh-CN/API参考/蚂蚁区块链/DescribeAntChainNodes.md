# DescribeAntChainNodes {#doc_api_Baas_DescribeAntChainNodes .reference}

查询一条蚂蚁区块链的节点信息列表

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainNodes&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|1q8B5R9p|区块链ID

 |
|Action|String|否|DescribeAntChainNodes|系统规定参数。取值：DescribeAntChainNodes。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|BA9738FE-F427-44FD-A1D9-EB4EFB43075A|请求ID

 |
|Result| |\[\]|请求结果

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainNodes
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"BA9738FE-F427-44FD-A1D9-EB4EFB43075A",
	"data":{
		"Result":[
			{
				"publicKey":"0x9934CFA59EE6CB241AEC242411BCD67D1DA8E07095FFC49DCB1102F2625031EBE9636CD6C392F675214E406C9AA55CD7F8A9EA11BD54C93258FA93BED717EACD",
				"nodeId":"0x79233E99716D28740AA00CFE0C1274C34C9E5511EE910C227999683EAF749553",
				"nodeState":2,
				"endpoints":[
					{
						"port":"18130",
						"ip":"47.101.74.49"
					}
				],
				"nodeType":1
			},
			{
				"publicKey":"0x63F4F303751FB86866718A4C797CE4CD8DDBECCB2E113D5CB9B41818C6C549FEA9E559601916F0F4BDCABDC16C170ECAFA0525C8345490161124EC8386F39B93",
				"nodeId":"0x9E953C89ADA2E927F7EAE866D2F26828B330D44DD17FEA84195B902B1AD1D1B1",
				"nodeState":2,
				"endpoints":[
					{
						"port":"18131",
						"ip":"47.101.74.49"
					}
				],
				"nodeType":1
			},
			{
				"publicKey":"0x1143C35FEFF1EB151AEB77C19A6ECC6FFD6BA13AA1913C60A9ADACA08AA6CB51A555ACF6E3E6B658142EB464EF2199AE41CA0EC5ACEB6514B5F56E2D2395CE78",
				"nodeId":"0x77AD62D5041B92617488A0FDD8E341C06352344FA09F614AD7FDF616C1936B92",
				"nodeState":2,
				"endpoints":[
					{
						"port":"18132",
						"ip":"47.101.74.49"
					}
				],
				"nodeType":1
			},
			{
				"publicKey":"0xCD15C9C87DAB460C2F4AE48752E98AF023B8810777CAAA563E045EF04F714A8D2934998CAC00F462C81EB23B3816D39E07B81B49695FEA827342FDCEA982E3B6",
				"nodeId":"0x3F6355C92FB81904A1D9FD6E7781415A2B4455704BCFE2A8A0466302BD8EA5C8",
				"nodeState":2,
				"endpoints":[
					{
						"port":"18133",
						"ip":"47.101.74.49"
					}
				],
				"nodeType":1
			}
		],
		"RequestId":"BA9738FE-F427-44FD-A1D9-EB4EFB43075A"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

