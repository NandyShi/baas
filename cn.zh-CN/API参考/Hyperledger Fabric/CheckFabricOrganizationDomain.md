# CheckFabricOrganizationDomain {#doc_api_Baas_CheckFabricOrganizationDomain .reference}

调用CheckFabricOrganizationDomain检查域名是否可用。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CheckFabricOrganizationDomain&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|CheckFabricOrganizationDomain|系统规定参数。取值：**CheckFabricOrganizationDomain**。

 |
|Domain|String|否|bank|域名前缀。

 不需要包含`DescribeRootDomain`接口获取的根域名。

 |
|DomainCode|String|否|bank|域名。

 |
|RegionId|String|否|cn-hangzhou|地域。

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|ErrorCode|Integer|200|错误码

 |
|RequestId|String|C30A14C7-800E-468B-9EB2-C704DA49295E|请求ID

 |
|Result| | |检查结果

 |
|Domain|String|bank|返回用户输入的域名

 |
|Prompt|String|OK|提示

 |
|Valid|Boolean|true|是否有效

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CheckFabricOrganizationDomain
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<CheckFabricOrganizationDomainResponse>
	  <Result>
		    <Prompt>OK</Prompt>
		    <Domain>canyouguessme</Domain>
		    <Valid>true</Valid>
	  </Result>
	  <RequestId>C30A14C7-800E-468B-9EB2-C704DA49295E</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</CheckFabricOrganizationDomainResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"Prompt":"OK",
		"Domain":"canyouguessme",
		"Valid":true
	},
	"RequestId":"C30A14C7-800E-468B-9EB2-C704DA49295E",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

