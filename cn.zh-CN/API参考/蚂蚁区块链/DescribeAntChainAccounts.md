# DescribeAntChainAccounts {#doc_api_Baas_DescribeAntChainAccounts .reference}

查询一条蚂蚁区块链的账户列表

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainAccounts&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|pYogqb9v|区块链ID

 |
|PageNumber|Integer|是|1|页面编号

 |
|PageSize|Integer|是|10|每页数量

 |
|Action|String|否|DescribeAntChainAccounts|系统规定参数。取值：DescribeAntChainAccounts。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|1692940F-87C5-468F-8188-6C95FC05BBA5|请求ID

 |
|Result| | |请求结果

 |
|Accounts| | |账户信息

 |
|AccountPublicKey|String|de44334f1094cbd37e952ef691a837f36eab2e9afdf6bed9bf523c2dde40ff7b1ff526ec11b510d320f536685f75dd90f67fda8d41a69738a76a77c27b1373fb|账户公钥

 |
|AccountRecoveryKey|String|ee54a9c4511345f2de05889540eedb8dfed7b57ab0647c5894e4333596bc2ecef07a0469331d016ad9978b39367a0a5c217ef92ffffcbd6716db6667353891a9|账户恢复公钥

 |
|AccountStatus|String|NORMAL|状态

 |
|AntChainId|String|pYogqb9v|区块链ID

 |
|Pagination| | |分页信息

 |
|PageNumber|Integer|1|当前页面编号

 |
|PageSize|Integer|10|每页数量

 |
|TotalCount|Integer|1|总数

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainAccounts
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"1692940F-87C5-468F-8188-6C95FC05BBA5",
	"data":{
		"Result":{
			"Accounts":[
				{
					"AccountPublicKey":"de44334f1094cbd37e952ef691a837f36eab2e9afdf6bed9bf523c2dde40ff7b1ff526ec11b510d320f536685f75dd90f67fda8d41a69738a76a77c27b1373fb",
					"AccountStatus":"NORMAL",
					"AccountRecoveryKey":"ee54a9c4511345f2de05889540eedb8dfed7b57ab0647c5894e4333596bc2ecef07a0469331d016ad9978b39367a0a5c217ef92ffffcbd6716db6667353891a9",
					"Account":"账户名",
					"AntChainId":"pYogqb9v"
				}
			],
			"Pagination":{
				"PageNumber":1,
				"TotalCount":1,
				"PageSize":10
			}
		},
		"RequestId":"1692940F-87C5-468F-8188-6C95FC05BBA5"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

