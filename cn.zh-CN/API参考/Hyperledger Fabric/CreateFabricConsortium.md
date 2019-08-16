# CreateFabricConsortium {#doc_api_Baas_CreateFabricConsortium .reference}

调用CreateFabricConsortium创建联盟。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CreateFabricConsortium&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|CreateFabricConsortium|系统规定参数。取值：CreateFabricConsortium。

 |
|ChannelPolicy|String|是|Any|创建通道策略

 |
|ConsortiumName|String|是|aaaaa|联盟名

 |
|Domain|String|是|helloworld|域名

 |
|Location|String|是|cn-hangzhou|位置信息

 |
|OrdererType|String|是|Kafka|Orderer类型

 |
|SpecName|String|是|basic|规格

 |
|ConsortiumDescription|String|否|some|联盟描述

 |
|OrderersCount|Integer|否|2|Orderer数量

 |
|Organization.N.OrganizationId|String|否|peers-yidio-1tuigx42b1goc|组织ID

 |
|PaymentDuration|Integer|否|2|计费周期

 |
|PaymentDurationUnit|String|否|month|周期单位

 |
|PeersCount|Integer|否|2|Peer数量

 |
|RegionId|String|否|cn-hangzhou|地域

 |
|ZoneId|String|否|random|区域

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
|ChannelCount|Integer|0|通道数量

 |
|ChannelPolicy|String|Any|通道策略

 |
|ClusterState|String|Pending|集群状态

 |
|CodeName|String|lianmenyumingyi|域名

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

 |
|ConsortiumName|String|myconsortium|联盟名

 |
|CreateTime|String|1544086901984|创建时间

 |
|Description|String|string|描述

 |
|Domain|String|hello|域名

 |
|MemberCount|Integer|2|成员数量

 |
|OrdererCount|Integer|1|orderer数量

 |
|OrdererType|String|Kafka|orderer类型

 |
|OwnerBid|String|26842|创建者bid

 |
|OwnerUid|Long|1019556|创建者uid

 |
|RegionId|String|cn-hangzhou|地域

 |
|ServiceState|String|Pending|服务状态

 |
|SpecName|String|basic|规格

 |
|ZoneId|String|cn-hangzhou|区域

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CreateFabricConsortium
&ChannelPolicy=Any
&ConsortiumName=aaaaa
&Domain=helloworld
&Location=cn-hangzhou
&OrdererType=Kafka
&SpecName=basic
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<CreateFabricConsortiumResponse>
  <result>
		    <CodeName>阿里巴巴集团区块链联盟</CodeName>
		    <ClusterState>Pending</ClusterState>
		    <ConsortiumId>c-93k8d34jy79y79</ConsortiumId>
		    <CreateTime>1999-05-10 09:00:00</CreateTime>
		    <OwnerBid>12312</OwnerBid>
		    <OrdererCount>1</OrdererCount>
		    <OrdererType>kafka</OrdererType>
		    <ConsortiumName>阿里巴巴集团</ConsortiumName>
		    <OrganizationCount>3</OrganizationCount>
		    <ChannelCount>0</ChannelCount>
		    <ChannelPolicy>ANY</ChannelPolicy>
		    <Description>string</Description>
		    <Domain>domain</Domain>
		    <MemberCount>2</MemberCount>
		    <ServiceState>Pending</ServiceState>
	  </result>
	  <RequestId>2537DB1B-F478-431E-A847-5DDAAE2BD251</RequestId>
	  <ErrorCode>200</ErrorCode>
	  <Success>true</Success>
</CreateFabricConsortiumResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"result":{
		"ConsortiumName":"阿里巴巴集团",
		"Description":"string",
		"ConsortiumId":"c-93k8d34jy79y79",
		"Domain":"domain",
		"OrganizationCount":3,
		"OwnerBid":12312,
		"ChannelCount":0,
		"ClusterState":"Pending",
		"CreateTime":"1999-05-10 09:00:00",
		"CodeName":"阿里巴巴集团区块链联盟",
		"OrdererType":"kafka",
		"ServiceState":"Pending",
		"MemberCount":2,
		"OrdererCount":1,
		"ChannelPolicy":"ANY"
	},
	"RequestId":"2537DB1B-F478-431E-A847-5DDAAE2BD251",
	"Success":true,
	"ErrorCode":200
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

