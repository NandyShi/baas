# CreateFabricOrganizationUser {#doc_api_Baas_CreateFabricOrganizationUser .reference}

调用CreateFabricOrganizationUser创建组织用户。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CreateFabricOrganizationUser&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|CreateFabricOrganizationUser|系统规定参数。取值：**CreateFabricOrganizationUser**。

 |
|OrganizationId|String|是|peers-yidio-1tuigx42b\*\*\*\*|组织ID

 |
|Username|String|是|username|用户名

 |
|Attrs|String|否|foo=foo1,bar=bar1|ABAC属性

 |
|Password|String|否|password|密码

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
|CreateTime|String|1544086901984|创建时间

 |
|ExpireTime|String|1544411108000|过期时间

 |
|Fullname|String|fullname|全名

 |
|OrganizationId|String|peers-yidio-1tuigx42b\*\*\*\*|组织ID

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

http(s)://[Endpoint]/?Action=CreateFabricOrganizationUser
&OrganizationId=peers-yidio-1tuigx42b****
&Username=username
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<CreateFabricOrganizationUserResponse>
	  <result>
		    <OrganizationId>peers-yidio-1tuigx42b****</OrganizationId>
		    <CreateTime>1999-05-10 09:00:00</CreateTime>
		    <ExpireTime>2000-05-10 09:00:00</ExpireTime>
		    <Fullname>阿里巴巴集团</Fullname>
		    <Username>username</Username>
		    <Password>pwd</Password>
	  </result>
	  <RequestId>2537DB1B-F478-431E-A847-5DDAAE2BD251</RequestId>
	  <ErrorCode>200</ErrorCode>
	  <Success>true</Success>
</CreateFabricOrganizationUserResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"result":{
		"Fullname":"阿里巴巴集团",
		"ExpireTime":"2000-05-10 09:00:00",
		"Password":"pwd",
		"Username":"username",
		"CreateTime":"1999-05-10 09:00:00",
		"OrganizationId":"peers-yidio-1tuigx42b****"
	},
	"RequestId":"2537DB1B-F478-431E-A847-5DDAAE2BD251",
	"Success":true,
	"ErrorCode":200
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

