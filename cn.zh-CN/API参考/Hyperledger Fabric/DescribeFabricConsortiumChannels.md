# DescribeFabricConsortiumChannels {#doc_api_Baas_DescribeFabricConsortiumChannels .reference}

调用DescribeFabricConsortiumChannels获取联盟的通道列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricConsortiumChannels&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricConsortiumChannels|系统规定参数。取值：**DescribeFabricConsortiumChannels**。

 |
|ConsortiumId|String|是|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

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
|Result| | |联盟的通道列表

 |
|BatchTimeout|Integer|2|批处理超时时间

 |
|BlockCount|Integer|2|块数量

 |
|ChaincodeCount|Integer|2|链码数量

 |
|ChannelId|String|chan-channelx-1l1hmckuuisxo|通道ID

 |
|ChannelName|String|mychammel|通道名

 |
|ConsortiumChannelId|Integer|1|联盟中通道序列

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

 |
|ConsortiumName|String|name|联盟名

 |
|CreateTime|String|1544411108000|创建时间

 |
|DeleteTime|String|1544411108000|删除时间

 |
|Deleted|Boolean|true|是否删除

 |
|MaxMessageCount|Integer|200|块包含最大消息条目

 |
|MemberCount|Integer|3|通道成员数量

 |
|MemberJoinedCount|String|3|加入联盟的成员数量

 |
|NeedJoined|Boolean|true|是否需要加入

 |
|OwnerBid|String|26842|创建者Bid

 |
|OwnerName|String|uid-\*|创建者

 |
|OwnerUid|Integer|212|创建者Uid

 |
|PreferredMaxBytes|Integer|102410241|首选最大字节数

 |
|RequestId|String|1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3|请求ID

 |
|State|String|Running|状态

 |
|SupportChannelConfig|Boolean|true|是否支持自定义配置参数

 |
|UpdateTime|String|1544411108000|更新时间

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricConsortiumChannels
&ConsortiumId=consortium-lianmenyumingyi-hc5d1bwlulg7
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricConsortiumChannelsResponse>
  <result>
		    <BatchTimeout>2</BatchTimeout>
		    <BlockCount>2</BlockCount>
		    <ChaincodeCount>2</ChaincodeCount>
		    <ChannelId>chan-channelx-1l1hmckuuisxo</ChannelId>
		    <ChannelName>mychannel</ChannelName>
		    <ConsortiumId>consortium-lianmenyumingyi-hc5d1bwlulg7</ConsortiumId>
		    <ConsortiumName>name</ConsortiumName>
		    <CreateTime>1544411108000</CreateTime>
		    <DeleteTime>1544411108000</DeleteTime>
		    <Deleted>true</Deleted>
		    <OwnerBid>26842</OwnerBid>
		    <OwnerUid>212</OwnerUid>
		    <PreferredMaxBytes>12356</PreferredMaxBytes>
		    <State>Running</State>
		    <SupportChannelConfig>true</SupportChannelConfig>
		    <UpdateTime>1544411108000</UpdateTime>
	  </result>
	  <RequestId>2537DB1B-F478-431E-A847-5DDAAE2BD251</RequestId>
	  <ErrorCode>200</ErrorCode>
	  <Success>true</Success>
</DescribeFabricConsortiumChannelsResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"result":{
		"ConsortiumName":"name",
		"Deleted":"true",
		"ConsortiumId":"consortium-lianmenyumingyi-hc5d1bwlulg7",
		"UpdateTime":"1544411108000",
		"ChannelName":"mychannel",
		"ChaincodeCount":2,
		"OwnerBid":"26842",
		"ChannelId":"chan-channelx-1l1hmckuuisxo",
		"BlockCount":2,
		"DeleteTime":"1544411108000",
		"OwnerUid":212,
		"State":"Running",
		"BatchTimeout":2,
		"SupportChannelConfig":"true",
		"CreateTime":"1544411108000",
		"PreferredMaxBytes":12356
	},
	"RequestId":"2537DB1B-F478-431E-A847-5DDAAE2BD251",
	"Success":true,
	"ErrorCode":200
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

