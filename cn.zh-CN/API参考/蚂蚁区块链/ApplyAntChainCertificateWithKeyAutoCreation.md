# ApplyAntChainCertificateWithKeyAutoCreation {#doc_api_Baas_ApplyAntChainCertificateWithKeyAutoCreation .reference}

申请链接一条蚂蚁区块链，自动生成证书等连接信息

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=ApplyAntChainCertificateWithKeyAutoCreation&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|1q8B5R9p|区块链ID

 |
|CommonName|String|是|commonName|通用名称（CN）

 |
|ConsortiumId|String|是|DV80nJXq|联盟ID

 |
|CountryName|String|是|countryName|城市名（L）

 |
|LocalityName|String|是|localityName|国家名（C）

 |
|OrganizationName|String|是|organizationName|机构名（O）

 |
|OrganizationUnitName|String|是|organizationUnitName|组织单位名（OU）

 |
|Password|String|是|password|SSL密钥密码

 |
|StateOrProvinceName|String|是|stateOrProvinceName|省名（ST）

 |
|Action|String|否|ApplyAntChainCertificateWithKeyAutoCreation|系统规定参数。取值：ApplyAntChainCertificateWithKeyAutoCreation。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|3E1894AF-FEE7-4C6C-8C2A-2B3EE0105B07|请求ID

 |
|Result| | |请求结果

 |
|DownloadPath| | |下载地址

 |
|CaCrtUrl|String|http://\*\*\*ca.crt|ca.crt下载链接

 |
|ClientCrtUrl|String|http://\*\*\*client.crt|client.crt下载链接

 |
|SdkUrl|String|http://\*\*\*|sdk下载链接

 |
|TrustCaUrl|String|http://\*\*\*trustCa|trustCA下载链接

 |
|PrivateKey|String|-----BEGIN ENCRYPTED PRIVATE KEY-----\\nMII\*\*\*A=\\n-----END ENCRYPTED PRIVATE KEY-----\\n|私钥

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=ApplyAntChainCertificateWithKeyAutoCreation
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"3E1894AF-FEE7-4C6C-8C2A-2B3EE0105B07",
	"data":{
		"Result":{
			"DownloadPath":{
				"SdkUrl":"http://***",
				"TrustCaUrl":"http://***trustCa",
				"CaCrtUrl":"http://***ca.crt",
				"ClientCrtUrl":"http://***client.crt"
			},
			"PrivateKey":"-----BEGIN ENCRYPTED PRIVATE KEY-----\nMII***A=\n-----END ENCRYPTED PRIVATE KEY-----\n"
		},
		"RequestId":"3E1894AF-FEE7-4C6C-8C2A-2B3EE0105B07"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

