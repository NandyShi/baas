# CreateFabricOrganization {#doc_api_Baas_CreateFabricOrganization .reference}

调用CreateFabricOrganization创建组织。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CreateFabricOrganization&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|CreateFabricOrganization|系统规定参数。取值：**CreateFabricOrganization**。

 |
|Domain|String|是|domain|域名

 |
|Location|String|是|cn-hangzhou|区域

 |
|OrganizationName|String|是|name|名称

 |
|SpecName|String|是|basic|规格名

 |
|Description|String|否|description|描述

 |
|PaymentDuration|Integer|否|12|计费周期

 |
|PaymentDurationUnit|String|否|2|周期单位

 |
|PeersCount|Integer|否|2|节点数据量

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
|ClusterState|String|Pending|集群状态

 |
|CodeName|String|name|域名代码

 |
|ConsortiumCount|Integer|2|联盟数量

 |
|CreateTime|String|1544086901984|创建时间

 |
|Domain|String|domain|域名

 |
|OrganizationDescription|String|desc|组织描述

 |
|OrganizationId|String|zuzhiyumingyi-hc5d1bwlulg7|组织ID

 |
|OrganizationName|String|zuzhiyumingyi|组织名称

 |
|OwnerBid|String|26842|所有者业务代码

 |
|OwnerName|String|name|所有者名称

 |
|OwnerUid|Integer|1019556|所有者用户ID

 |
|PeerCount|Integer|3|组织节点数目

 |
|RegionId|String|cn-hangzhou|组织节点所在区域

 |
|RequestId|String|1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3|请求ID

 |
|ServiceState|String|Pending|服务状态

 |
|SpecName|String|baisc|节点规格

 |
|UserCount|Integer|2|组织用户数

 |
|ZoneId|String|zone|组织节点所在可用区

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CreateFabricOrganization
&Domain=domain
&Location=cn-hangzhou
&OrganizationName=name
&SpecName=basic
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<CreateFabricOrganizationResponse>
	  <result>
		    <CodeName>阿里巴巴集团区块链联盟</CodeName>
		    <ClusterState>Pending</ClusterState>
		    <OrganizationId>c-93k8d34jy79y79</OrganizationId>
		    <CreateTime>1999-05-10 09:00:00</CreateTime>
		    <OwnerBid>12312</OwnerBid>
		    <OrganizationName>阿里巴巴集团</OrganizationName>
		    <SpecName>basic</SpecName>
		    <ConsortiumCount>0</ConsortiumCount>
		    <PeerCount>3</PeerCount>
		    <Description>string</Description>
		    <Domain>domain</Domain>
		    <UserCount>2</UserCount>
		    <ServiceState>Pending</ServiceState>
	  </result>
	  <RequestId>2537DB1B-F478-431E-A847-5DDAAE2BD251</RequestId>
	  <ErrorCode>200</ErrorCode>
	  <Success>true</Success>
</CreateFabricOrganizationResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"result":{
		"Description":"string",
		"Domain":"domain",
		"OrganizationId":"c-93k8d34jy79y79",
		"OwnerBid":12312,
		"OrganizationName":"阿里巴巴集团",
		"ClusterState":"Pending",
		"ConsortiumCount":0,
		"UserCount":2,
		"SpecName":"basic",
		"CreateTime":"1999-05-10 09:00:00",
		"CodeName":"阿里巴巴集团区块链联盟",
		"PeerCount":3,
		"ServiceState":"Pending"
	},
	"RequestId":"2537DB1B-F478-431E-A847-5DDAAE2BD251",
	"Success":true,
	"ErrorCode":200
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

