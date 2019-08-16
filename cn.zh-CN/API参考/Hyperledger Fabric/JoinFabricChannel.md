# JoinFabricChannel {#doc_api_Baas_JoinFabricChannel .reference}

调用JoinFabricChannel确认加入通道。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=JoinFabricChannel&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|JoinFabricChannel|系统规定参数。取值：**JoinFabricChannel**。

 |
|ChannelId|String|是|chan-channelx-1l1hmckuu\*\*\*\*|通道ID

 |
|Do|String|是|accept|操作

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
|Result| | |结果

 |
|AcceptTime|String|1533025590|接受时间

 |
|ApproveTime|String|1533025590|批准时间

 |
|ChannelId|String|channelid|通道ID

 |
|ConfirmTime|String|1533025590|确认时间

 |
|DestroyTime|String|1533025590|销毁时间

 |
|InviteTime|String|1533025590|邀请时间

 |
|OrganizationId|String|peers-aaaaaa2-1eqnj5o5w9dt3|组织ID

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

http(s)://[Endpoint]/?Action=JoinFabricChannel
&ChannelId=chan-channelx-1l1hmckuu****
&Do=accept
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<JoinFabricChannelResponse>
	  <Result>
		    <InviteTime>2018-06-21T13:41:48.000+0000</InviteTime>
		    <ChannelId>ch-2n5fgcikopo4al</ChannelId>
		    <WithPeer>true</WithPeer>
		    <ApproveTime>2018-06-21T13:41:48.000+0000</ApproveTime>
		    <ConfirmTime>2018-06-21T13:41:48.000+0000</ConfirmTime>
		    <DestroyTime>2018-06-21T13:41:48.000+0000</DestroyTime>
		    <State>Accepted</State>
		    <OrganizationId>org1</OrganizationId>
		    <AcceptTime>2018-06-21T13:41:48.000+0000</AcceptTime>
	  </Result>
	  <RequestId>7D27692E-C501-4B1D-878C-0B869DD3D9E6</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</JoinFabricChannelResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"ChannelId":"ch-2n5fgcikopo4al",
		"InviteTime":"2018-06-21T13:41:48.000+0000",
		"WithPeer":true,
		"State":"Accepted",
		"ApproveTime":"2018-06-21T13:41:48.000+0000",
		"ConfirmTime":"2018-06-21T13:41:48.000+0000",
		"OrganizationId":"org1",
		"DestroyTime":"2018-06-21T13:41:48.000+0000",
		"AcceptTime":"2018-06-21T13:41:48.000+0000"
	},
	"RequestId":"7D27692E-C501-4B1D-878C-0B869DD3D9E6",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

