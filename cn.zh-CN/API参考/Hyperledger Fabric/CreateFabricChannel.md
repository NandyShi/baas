# CreateFabricChannel {#doc_api_Baas_CreateFabricChannel .reference}

调用CreateFabricChannel创建通道。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CreateFabricChannel&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|CreateFabricChannel|系统规定参数。取值：**CreateFabricChannel**。

 |
|ChannelName|String|是|channelx|通道名。最大长度50个字符，可以包含英文或数字及符号"\_", "-", "."。

 |
|ConsortiumId|String|是|consortium-aaaaaa-akpcsjjac2jd|联盟ID。

 |
|BatchTimeout|Integer|否|2|块超时时间。

 |
|MaxMessageCount|Integer|否|50|块交易上限。

 |
|Organization.N.Id|String|否|peers-aaaaaa1-1oxw31d046jtl|加入通道的组织ID号列表，输入：`Organization.1.Id=org1&Organization.2.Id=org2`。

 |
|PreferredMaxBytes|Integer|否|12|块大小软限制。

 |
|RegionId|String|否|cn-hangzhou|地域。

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|ErrorCode|Integer|200|错误码

 |
|RequestId|String|1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3|请求ID

 |
|Result| | |创建结果

 |
|BatchTimeout|Integer|2|块超时时间

 |
|BlockCount|Integer|2|块个数

 |
|ChaincodeCount|Integer|2|链码数量

 |
|ChannelId|String|chan-channelx-1l1hmckuuisxo|通道ID

 |
|ChannelName|String|channelx|通道名

 |
|ConsortiumId|String|consortium-aaaaaa-akpcsjjac2jd|联盟ID

 |
|ConsortiumName|String|aaaaaa|联盟名

 |
|CreateTime|String|1544768139624|创建时间

 |
|MaxMessageCount|Integer|50|块交易上限

 |
|MemberCount|Integer|1|成员数量

 |
|OwnerBid|String|26842|创建者Bid

 |
|OwnerName|String|uid-|创建者

 |
|OwnerUid|Integer|1234|创建者Uid

 |
|PreferredMaxBytes|Integer|12|块大小软限制

 |
|RequestId|String|1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3|请求ID

 |
|State|String|Running|状态

 |
|SupportConfig|Boolean|true|是否支持配置

 |
|UpdateTime|String|1544768139624|更新时间

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CreateFabricChannel
&ChannelName=channelx
&ConsortiumId=consortium-aaaaaa-akpcsjjac2jd
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<CreateFabricChannelResponse>
	  <Result>
		    <ChannelId>chan-channelx-1l1hmckuuisxo</ChannelId>
		    <ConsortiumName>aaaaa</ConsortiumName>
		    <ChannelName>channelx</ChannelName>
		    <ConsortiumId>consortium-aaaaaa-akpcsjjac2jd</ConsortiumId>
		    <CreateTime>1544768139624</CreateTime>
		    <MaxMessageCount>50</MaxMessageCount>
		    <MemberCount>2</MemberCount>
		    <OwnerBid>26842</OwnerBid>
		    <OwnerUid></OwnerUid>
		    <OwnerName>name</OwnerName>
		    <PreferredMaxBytes>12</PreferredMaxBytes>
		    <State>Pending</State>
		    <SupportConfig>true</SupportConfig>
		    <UpdateTime>1544768139624</UpdateTime>
	  </Result>
	  <RequestId></RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</CreateFabricChannelResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"ConsortiumName":"aaaaa",
			"ConsortiumId":"consortium-aaaaaa-akpcsjjac2jd",
			"UpdateTime":"1544768139624",
			"ChannelName":"channelx",
			"MaxMessageCount":50,
			"SupportConfig":"true",
			"OwnerBid":"26842",
			"ChannelId":"chan-channelx-1l1hmckuuisxo",
			"OwnerUid":"",
			"State":"Pending",
			"CreateTime":"1544768139624",
			"PreferredMaxBytes":12,
			"MemberCount":2,
			"OwnerName":"name"
		}
	],
	"RequestId":"",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

