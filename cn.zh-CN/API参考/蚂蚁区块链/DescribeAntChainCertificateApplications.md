# DescribeAntChainCertificateApplications {#doc_api_Baas_DescribeAntChainCertificateApplications .reference}

查看联盟成员申请连接一条蚂蚁区块链的信息

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainCertificateApplications&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|1q8B5R9p|区块链ID

 |
|PageNumber|Integer|是|1|页面编号

 |
|PageSize|Integer|是|20|每页数量

 |
|Status|String|是|1|状态

 |
|Action|String|否|DescribeAntChainCertificateApplications|系统规定参数。取值：DescribeAntChainCertificateApplications。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|B232A84E-7944-4EB0-83D0-9D409E12E0A8|请求ID

 |
|Result| | |请求结果

 |
|CertificateApplications| | |证书申请信息

 |
|AntChainId|String|1q8B5R9p|区块链ID

 |
|Bid|String|26842|Bid

 |
|Createtime|Long|1563949275000|创建时间

 |
|Status|String|1|状态

 |
|Updatetime|Long|1563949275000|更新时间

 |
|Username|String|uid-1287126353308684|账户名

 |
|Pagination| | |分页信息

 |
|PageNumber|Integer|1|页面数

 |
|PageSize|Integer|20|每页数量

 |
|TotalCount|Integer|1|每页总量

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainCertificateApplications
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"B232A84E-7944-4EB0-83D0-9D409E12E0A8",
	"data":{
		"Result":{
			"CertificateApplications":[
				{
					"Status":1,
					"Username":"uid-1287126353308684",
					"Bid":"26842",
					"AntChainId":"1q8B5R9p",
					"Createtime":1563949275000,
					"Updatetime":1563949275000
				}
			],
			"Pagination":{
				"PageNumber":1,
				"TotalCount":1,
				"PageSize":20
			}
		},
		"RequestId":"B232A84E-7944-4EB0-83D0-9D409E12E0A8"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

