# DescribeFabricOrganizationDeletable {#doc_api_Baas_DescribeFabricOrganizationDeletable .reference}

调用DescribeFabricOrganizationDeletable查询组织是否可删除。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricOrganizationDeletable&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|OrganizationId|String|是|peers-aaaaaa2-1eqnj5o5w\*\*\*\*|组织ID

 |
|Action|String|否|DescribeFabricOrganizationDeletable|系统规定参数。取值：**DescribeFabricOrganizationDeletable**。

 |
|Location|String|否|cn-hangzhou|位置信息

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
|CodeName|String|name|域名前缀

 |
|Deletable|Boolean|true|是否可删除

 |
|Domain|String|domain|域名

 |
|OrganizationDescription|String|desc|组织描述

 |
|OrganizationId|String|peers-aaaaaa2-1eqnj5o5w\*\*\*\*|组织ID

 |
|OrganizationName|String|orgname|组织名

 |
|RegionId|String|cn-hangzhou|地域

 |
|State|String|Running|状态

 |
|ZoneId|String|zone|可用区

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricOrganizationDeletable
&OrganizationId=peers-aaaaaa2-1eqnj5o5w****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricOrganizationDeletableResponse>
	  <Result>
		    <Deletable>true</Deletable>
		    <OrganizationId>consortium-xxxxxx</OrganizationId>
		    <CodeName>name</CodeName>
		    <Domain>domain</Domain>
		    <OrganizationDescription>desc</OrganizationDescription>
		    <OrganizationName>orgname</OrganizationName>
		    <RegionId>cn-hangzhou</RegionId>
		    <State>Running</State>
		    <ZoneId>zone</ZoneId>
	  </Result>
	  <RequestId>C445762C-8909-4BD8-A2BD-BB45BF2441D8</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricOrganizationDeletableResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"OrganizationDescription":"desc",
		"State":"Running",
		"Domain":"domain",
		"RegionId":"cn-hangzhou",
		"CodeName":"name",
		"ZoneId":"zone",
		"OrganizationId":"consortium-xxxxxx",
		"Deletable":true,
		"OrganizationName":"orgname"
	},
	"RequestId":"C445762C-8909-4BD8-A2BD-BB45BF2441D8",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

