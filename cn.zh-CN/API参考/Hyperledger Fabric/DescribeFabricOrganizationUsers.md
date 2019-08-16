# DescribeFabricOrganizationUsers {#doc_api_Baas_DescribeFabricOrganizationUsers .reference}

调用DescribeFabricOrganizationUsers获取组织的用户列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricOrganizationUsers&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricOrganizationUsers|系统规定参数。取值：**DescribeFabricOrganizationUsers**。

 |
|OrganizationId|String|是|peers-aaaaaa2-1eqnj5o5w\*\*\*\*|组织ID

 |
|Location|String|否|cn-hangzhou|位置

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
|Result| | |组织的用户列表

 |
|Attrs|String|foo=foo1,bar=bar1|ABAC属性

 |
|CallerBid|String|26842|调用者业务ID

 |
|CallerUid|Long|111111111111|调用者用户ID

 |
|CreateTime|String|1533025590|创建时间

 |
|ExpireTime|String|1533025590|过期时间

 |
|FullName|String|name|全名

 |
|OrganizationId|String|peers-aaaaaa2-1eqnj5o5w9dt3|组织ID

 |
|RegionId|String|cn-hangzhou|地域ID

 |
|Username|String|username|用户名

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricOrganizationUsers
&OrganizationId=peers-aaaaaa2-1eqnj5o5w****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricOrganizationUsersResponse>
	  <result>
		    <Attrs>foo=foo1,bar=bar1</Attrs>
		    <Username>username</Username>
		    <OrganizationId>peers-aaaaaa2-1eqnj5o5w9dt3</OrganizationId>
		    <ChannelName>mychannel</ChannelName>
		    <CreateTime>1544411108000</CreateTime>
		    <ExpireTime>1544411108000</ExpireTime>
		    <CallerBid>26842</CallerBid>
		    <CallerUid>212</CallerUid>
	  </result>
	  <RequestId>2537DB1B-F478-431E-A847-5DDAAE2BD251</RequestId>
	  <ErrorCode>200</ErrorCode>
	  <Success>true</Success>
</DescribeFabricOrganizationUsersResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"result":{
		"CallerUid":212,
		"ExpireTime":"1544411108000",
		"CreateTime":"1544411108000",
		"Username":"username",
		"Attrs":"foo=foo1,bar=bar1",
		"CallerBid":"26842",
		"ChannelName":"mychannel",
		"OrganizationId":"peers-aaaaaa2-1eqnj5o5w9dt3"
	},
	"RequestId":"2537DB1B-F478-431E-A847-5DDAAE2BD251",
	"Success":true,
	"ErrorCode":200
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

