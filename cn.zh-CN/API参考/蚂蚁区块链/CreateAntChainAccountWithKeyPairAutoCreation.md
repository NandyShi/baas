# CreateAntChainAccountWithKeyPairAutoCreation {#doc_api_Baas_CreateAntChainAccountWithKeyPairAutoCreation .reference}

在一条蚂蚁区块链上创建一个账户，通过自动生成keypair 的方式

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CreateAntChainAccountWithKeyPairAutoCreation&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Account|String|否|accountname|账户名称

 |
|Action|String|否|CreateAntChainAccountWithKeyPairAutoCreation|系统规定参数。取值：CreateAntChainAccountWithKeyPairAutoCreation。

 |
|AntChainId|String|否|1q8B5R9p|区块链ID

 |
|Password|String|否|password|密码

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|5F058BB4-3043-4638-86D4-EED84AD1AE54|请求ID

 |
|Result| | |请求结果

 |
|Account|String|accountname|账户名

 |
|AccountPrivateKey|String|-----BEGIN ENCRYPTED PRIVATE KEY-----\\nM\*\*\*8=\\n-----END ENCRYPTED PRIVATE KEY-----\\n|账户私钥

 |
|AccountPublicKey|String|b\*\*\*7|账户公钥

 |
|AccountRecoverPrivateKey|String|-----BEGIN ENCRYPTED PRIVATE KEY-----\\nM\*\*\*Io=\\n-----END ENCRYPTED PRIVATE KEY-----\\n|账户恢复私钥

 |
|AccountRecoverPublicKey|String|d\*\*\*b|账户恢复公钥

 |
|AntChainId|String|1q8B5R9p|区块链ID

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CreateAntChainAccountWithKeyPairAutoCreation
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"5F058BB4-3043-4638-86D4-EED84AD1AE54",
	"data":{
		"Result":{
			"AccountRecoverPrivateKey":"-----BEGIN ENCRYPTED PRIVATE KEY-----\nM***Io=\n-----END ENCRYPTED PRIVATE KEY-----\n",
			"AccountPublicKey":"b***7",
			"AccountRecoverPublicKey":"d***b",
			"AccountPrivateKey":"-----BEGIN ENCRYPTED PRIVATE KEY-----\nM***8=\n-----END ENCRYPTED PRIVATE KEY-----\n",
			"Account":"accountname",
			"AntChainId":"1q8B5R9p"
		},
		"RequestId":"5F058BB4-3043-4638-86D4-EED84AD1AE54"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

