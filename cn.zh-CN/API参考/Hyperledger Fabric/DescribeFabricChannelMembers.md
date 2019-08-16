# DescribeFabricChannelMembers {#doc_api_Baas_DescribeFabricChannelMembers .reference}

调用DescribeFabricChannelMembers查询通道的成员列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricChannelMembers&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricChannelMembers|系统规定参数。取值：**DescribeFabricChannelMembers**。

 |
|ChannelId|String|是|chan-channelx-1l1hmckuu\*\*\*\*|通道ID

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
|Result| | |通道的成员列表

 |
|AcceptTime|String|1544411108000|接受时间

 |
|ChannelId|String|chan-channelx-1l1hmckuuisxo|通道ID

 |
|InviteTime|String|1544411108000|邀请时间

 |
|OrganizationDescription|String|description|组织描述

 |
|OrganizationDomain|String|hello|组织域名

 |
|OrganizationId|String|peers-aaaaaa1-1oxw31d046jtl|组织ID

 |
|OrganizationName|String|name|组织名

 |
|State|String|Running|状态

 |
|WithPeer|Boolean|true|是否包含节点

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricChannelMembers
&ChannelId=chan-channelx-1l1hmckuu****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricChannelMembersResponse>
	  <Result>
		    <OrganizationName>myorg</OrganizationName>
		    <InviteTime>2018-07-23T01:53:53.000+0000</InviteTime>
		    <ChannelId>chan-cc1-2f0l9cd394****</ChannelId>
		    <WithPeer>true</WithPeer>
		    <OrganizationDescription></OrganizationDescription>
		    <OrganizationDomain>zhuangADSADSDAACZXsdfadsdfaesfac1.absdasssample.cc</OrganizationDomain>
		    <State>Accepted</State>
		    <OrganizationId>peers-zhuang1-2kna27h5m3c913</OrganizationId>
		    <AcceptTime>2018-07-24T02:35:53.000+0000</AcceptTime>
	  </Result>
	  <RequestId>3E85A941-658C-40E8-9704-60513A0281CF</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricChannelMembersResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"ChannelId":"chan-cc1-2f0l9cd394****",
		"InviteTime":"2018-07-23T01:53:53.000+0000",
		"OrganizationDescription":"",
		"OrganizationDomain":"zhuangADSADSDAACZXsdfadsdfaesfac1.absdasssample.cc",
		"WithPeer":true,
		"State":"Accepted",
		"OrganizationId":"peers-zhuang1-2kna27h5m3c913",
		"AcceptTime":"2018-07-24T02:35:53.000+0000",
		"OrganizationName":"myorg"
	},
	"RequestId":"3E85A941-658C-40E8-9704-60513A0281CF",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

