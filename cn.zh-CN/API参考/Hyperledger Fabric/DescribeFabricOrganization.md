# DescribeFabricOrganization {#doc_api_Baas_DescribeFabricOrganization .reference}

调用DescribeFabricOrganization获取一个组织的详情。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricOrganization&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricOrganization|系统规定参数。取值：**DescribeFabricOrganization**。

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
|Result| | |组织的详细列表

 |
|CANAME|String|client|组织CA节点名称

 |
|CAUrl|String|https://ca1.org1.alibabacloudbaas.com:31154|组织CA节点地址

 |
|CodeName|String|org1|域名前缀

 |
|ConsortiumCount|Integer|2|联盟数

 |
|CreateTime|String|1533025590|创建时间

 |
|Domain|String|org1.alibabacloudbaas.com|域名

 |
|MSP|String|org1MSP|成员服务提供者

 |
|OrganizationDescription|String|This is org1|组织描述

 |
|OrganizationId|String|peers-aaaaaa2-1eqnj5o5w9dt3|组织ID

 |
|OrganizationName|String|org1|组织名称

 |
|OwnerBid|String|2544|创建者Bid

 |
|OwnerName|String|uid-23434|创建者

 |
|OwnerUid|Long|23434|创建者Uid

 |
|PeerCount|Integer|2|Peer节点数

 |
|RegionId|String|cn-hangzhou|地域

 |
|RequestId|String|1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3|请求ID

 |
|SpecName|String|basic|规格名

 |
|State|String|Running|状态

 |
|UserCount|Integer|2|用户数

 |
|ZoneId|String|cn-hangzhou-1a|可用区

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricOrganization
&OrganizationId=peers-aaaaaa2-1eqnj5o5w****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricOrganizationResponse>
  <Result>
		    <OrganizationDescription>organization created by ruiqi.zss</OrganizationDescription>
		    <Domain>peer.aliyun.abasssample.cc</Domain>
		    <ZoneId>cn-shanghai-a</ZoneId>
		    <OrganizationId>org-ip92i26m792c9</OrganizationId>
		    <OrganizationName>阿里云</OrganizationName>
		    <ConsortiumCount>1</ConsortiumCount>
		    <UserCount>0</UserCount>
		    <State>Created</State>
		    <SpecName>ecs.n1.medium</SpecName>
		    <OwnerUid>1204281570282129</OwnerUid>
		    <CAUrl>https://ca1.org1.alibabacloudbaas.com:31154</CAUrl>
		    <CreateTime>2018-06-22T06:14:21.000+0000</CreateTime>
		    <CANAME>caname</CANAME>
		    <CodeName>aliyun</CodeName>
		    <OwnerName>blockchain_baas_test</OwnerName>
		    <PeerCount>2</PeerCount>
		    <OwnerBid>26842</OwnerBid>
	  </Result>
	  <RequestId>C445762C-8909-4BD8-A2BD-BB45BF2441D8</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricOrganizationResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"Domain":"peer.aliyun.abasssample.cc",
		"CANAME":"caname",
		"ZoneId":"cn-shanghai-a",
		"CAUrl":"https://ca1.org1.alibabacloudbaas.com:31154",
		"OrganizationId":"org-ip92i26m792c9",
		"OwnerBid":"26842",
		"OrganizationName":"阿里云",
		"OrganizationDescription":"organization created by ruiqi.zss",
		"ConsortiumCount":1,
		"UserCount":0,
		"OwnerUid":1204281570282129,
		"State":"Created",
		"SpecName":"ecs.n1.medium",
		"CreateTime":"2018-06-22T06:14:21.000+0000",
		"CodeName":"aliyun",
		"PeerCount":2,
		"OwnerName":"blockchain_baas_test"
	},
	"RequestId":"C445762C-8909-4BD8-A2BD-BB45BF2441D8",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

