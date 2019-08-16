# ResetFabricOrganizationUserPassword {#doc_api_Baas_ResetFabricOrganizationUserPassword .reference}

调用ResetFabricOrganizationUserPassword重置用户密码。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=ResetFabricOrganizationUserPassword&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|ResetFabricOrganizationUserPassword|系统规定参数。取值：**ResetFabricOrganizationUserPassword**。

 |
|OrganizationId|String|是|peers-aaaaaa2-1eqnj5o5w\*\*\*\*|组织ID

 |
|Username|String|是|username|用户名

 |
|Location|String|否|cn-hangzhou|位置

 |
|Password|String|否|pwd|密码

 |
|RegionId|String|否|cn-hangzhou|地域

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|ErrorCode|Integer|200|错误码

 |
|RequestId|String|1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3|请求ID

 |
|Result| | |结果

 |
|CreateTime|String|1533025590|创建时间

 |
|ExpireTime|String|1533025590|过期时间

 |
|Fullname|String|username|全名

 |
|OrganizationId|String|peers-aaaaaa2-1eqnj5o5w\*\*\*\*|组织ID

 |
|Password|String|password|密码

 |
|Username|String|username|用户名

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=ResetFabricOrganizationUserPassword
&OrganizationId=peers-aaaaaa2-1eqnj5o5w****
&Username=username
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<ResetFabricOrganizationUserPasswordResponse>
	  <Result>
		    <Password>v32n9rzhxqk7</Password>
		    <CreateTime>1542086619000</CreateTime>
		    <ExpireTime>1542086619000</ExpireTime>
		    <Fullname>fullname</Fullname>
		    <Username>asian01</Username>
		    <OrganizationId>peers-asianbank-1c0w455jb****</OrganizationId>
	  </Result>
	  <RequestId>2A3ABD81-95F5-4931-ACB3-31BDAE561FC7</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</ResetFabricOrganizationUserPasswordResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"Fullname":"fullname",
		"ExpireTime":1542086619000,
		"Username":"asian01",
		"CreateTime":1542086619000,
		"Password":"v32n9rzhxqk7",
		"OrganizationId":"peers-asianbank-1c0w455jb****"
	},
	"RequestId":"2A3ABD81-95F5-4931-ACB3-31BDAE561FC7",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

