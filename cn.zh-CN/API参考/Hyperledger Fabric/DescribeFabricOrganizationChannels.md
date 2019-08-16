# DescribeFabricOrganizationChannels {#doc_api_Baas_DescribeFabricOrganizationChannels .reference}

调用DescribeFabricOrganizationChannels获取该组织加入的通道列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricOrganizationChannels&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricOrganizationChannels|系统规定参数。取值：**DescribeFabricOrganizationChannels**。

 |
|OrganizationId|String|是|peers-aaaaaa2-1eqnj5o5\*\*\*\*|组织ID

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
|Result| | |组织加入的通道列表

 |
|BatchTimeout|Integer|2|批处理超时时间

 |
|BlockCount|Integer|3|块数量

 |
|ChaincodeCount|Integer|2|链码数量

 |
|ChannelId|String|chan-channelx-1l1hmckuuisxo|通道ID

 |
|ChannelName|String|mychannel|通道名

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

 |
|ConsortiumName|String|name|联盟名称

 |
|CreateTime|String|1533025590|创建时间

 |
|DeleteTime|String|1533025590|删除时间

 |
|DeleteTime|String|1533025590|删除时间

 |
|Deleted|Boolean|true|是否已经删除

 |
|Deleted|Boolean|true|是否已经删除

 |
|MaxMessageCount|Integer|12|块包含最大消息条目

 |
|MemberCount|Integer|3|成员数量

 |
|OwnerBid|String|253|创建者Bid

 |
|OwnerName|String|uid-5324|创建者

 |
|OwnerUid|Integer|5324|创建者Uid

 |
|PreferredMaxBytes|Integer|24|首选最大字节数

 |
|RequestId|String|1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3|请求ID

 |
|State|String|Running|状态

 |
|SupportChannelConfig|Boolean|true|是否支持自定义配置参数

 |
|UpdateTime|String|1533025590|更新时间

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricOrganizationChannels
&OrganizationId=peers-aaaaaa2-1eqnj5o5****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricOrganizationChannelsResponse>
  <Result>
			    <ConsortiumName>perf914</ConsortiumName>
			    <Deleted>false</Deleted>
			    <ConsortiumId>consortium-perf914-37cfcff9pa2c7a</ConsortiumId>
			    <UpdateTime>2018-08-07T11:00:25.000+0000</UpdateTime>
			    <ChaincodeCount>18</ChaincodeCount>
			    <OwnerBid>26842</OwnerBid>
			    <ChannelId>chan-first-channel-31hlgpen5k5lig</ChannelId>
			    <Name>first-asdadaaaa aaaaaaaaaa dadscsdfasdasdafdscxzdwearq</Name>
			    <BlockCount>0</BlockCount>
			    <OwnerUid>1167481570282431</OwnerUid>
			    <DeleteTime></DeleteTime>
			    <State>Running</State>
			    <RequestId>23732B15-5165-4C85-8FFA-964C5D187AC2</RequestId>
			    <CreateTime>2018-08-07T11:00:25.000+0000</CreateTime>
			    <MemberCount>3</MemberCount>
			    <OwnerName>uid-1167481570282431</OwnerName>
		  </Result>
		  <Result>
			    <ConsortiumName>perf914</ConsortiumName>
			    <Deleted>false</Deleted>
			    <ConsortiumId>consortium-perf914-37cfcff9pa2c7a</ConsortiumId>
			    <UpdateTime>2018-08-08T08:05:52.000+0000</UpdateTime>
			    <ChaincodeCount>0</ChaincodeCount>
			    <OwnerBid>26842</OwnerBid>
			    <ChannelId>chan-yyp-1jpjolifn8g22k</ChannelId>
			    <Name>yyp</Name>
			    <BlockCount>0</BlockCount>
			    <OwnerUid>1167481570282431</OwnerUid>
			    <DeleteTime></DeleteTime>
			    <State>Running</State>
			    <RequestId>A6A0364C-FE54-4387-B44F-86D9A9BF346D</RequestId>
			    <CreateTime>2018-08-08T08:05:52.000+0000</CreateTime>
			    <MemberCount>1</MemberCount>
			    <OwnerName>uid-1167481570282431</OwnerName>
		  </Result>
		  <Result>
			    <ConsortiumName>perf914</ConsortiumName>
			    <Deleted>false</Deleted>
			    <ConsortiumId>consortium-perf914-37cfcff9pa2c7a</ConsortiumId>
			    <UpdateTime>2018-08-09T06:33:53.000+0000</UpdateTime>
			    <ChaincodeCount>7</ChaincodeCount>
			    <OwnerBid>26842</OwnerBid>
			    <ChannelId>chan-forthchannel-386gkfagakdgjl</ChannelId>
			    <Name>forthchannel</Name>
			    <BlockCount>0</BlockCount>
			    <OwnerUid>1167481570282431</OwnerUid>
			    <DeleteTime></DeleteTime>
			    <State>Running</State>
			    <RequestId>98BCF502-527C-4CDB-9C0A-BF2790295F27</RequestId>
			    <CreateTime>2018-08-09T06:33:53.000+0000</CreateTime>
			    <MemberCount>2</MemberCount>
			    <OwnerName>uid-1167481570282431</OwnerName>
		  </Result>
		  <RequestId>CAA5D19F-FB7A-4F69-AF1E-1BA37E9547C5</RequestId>
		  <Success>true</Success>
		  <ErrorCode>200</ErrorCode>
</DescribeFabricOrganizationChannelsResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"ConsortiumName":"perf914",
			"Deleted":false,
			"ConsortiumId":"consortium-perf914-37cfcff9pa2c7a",
			"UpdateTime":"2018-08-07T11:00:25.000+0000",
			"ChaincodeCount":18,
			"OwnerBid":"26842",
			"ChannelId":"chan-first-channel-31hlgpen5k5lig",
			"Name":"first-asdadaaaa aaaaaaaaaa dadscsdfasdasdafdscxzdwearq",
			"BlockCount":0,
			"OwnerUid":1167481570282431,
			"DeleteTime":"",
			"State":"Running",
			"CreateTime":"2018-08-07T11:00:25.000+0000",
			"RequestId":"23732B15-5165-4C85-8FFA-964C5D187AC2",
			"MemberCount":3,
			"OwnerName":"uid-1167481570282431"
		},
		{
			"ConsortiumName":"perf914",
			"Deleted":false,
			"ConsortiumId":"consortium-perf914-37cfcff9pa2c7a",
			"UpdateTime":"2018-08-08T08:05:52.000+0000",
			"ChaincodeCount":0,
			"OwnerBid":"26842",
			"ChannelId":"chan-yyp-1jpjolifn8g22k",
			"Name":"yyp",
			"BlockCount":0,
			"OwnerUid":1167481570282431,
			"DeleteTime":"",
			"State":"Running",
			"CreateTime":"2018-08-08T08:05:52.000+0000",
			"RequestId":"A6A0364C-FE54-4387-B44F-86D9A9BF346D",
			"MemberCount":1,
			"OwnerName":"uid-1167481570282431"
		},
		{
			"ConsortiumName":"perf914",
			"Deleted":false,
			"ConsortiumId":"consortium-perf914-37cfcff9pa2c7a",
			"UpdateTime":"2018-08-09T06:33:53.000+0000",
			"ChaincodeCount":7,
			"OwnerBid":"26842",
			"ChannelId":"chan-forthchannel-386gkfagakdgjl",
			"Name":"forthchannel",
			"BlockCount":0,
			"OwnerUid":1167481570282431,
			"DeleteTime":"",
			"State":"Running",
			"CreateTime":"2018-08-09T06:33:53.000+0000",
			"RequestId":"98BCF502-527C-4CDB-9C0A-BF2790295F27",
			"MemberCount":2,
			"OwnerName":"uid-1167481570282431"
		}
	],
	"RequestId":"CAA5D19F-FB7A-4F69-AF1E-1BA37E9547C5",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

