# DescribeFabricConsortiums {#doc_api_Baas_DescribeFabricConsortiums .reference}

调用DescribeFabricConsortiums获取联盟列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricConsortiums&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|否|DescribeFabricConsortiums|系统规定参数。取值：**DescribeFabricConsortiums**。

 |
|ConsortiumId|String|否|consortium-lianmenyumingyi-hc5d1bwl\*\*\*\*|联盟ID

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
|Result| | |联盟列表

 |
|ChannelCount|Integer|2|通道数

 |
|ChannelPolicy|String|Any|通道创建策略

 |
|CodeName|String|code|域名前缀

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwl\*\*\*\*|联盟ID

 |
|ConsortiumName|String|name|联盟名

 |
|CreateTime|String|1544411108000|创建时间

 |
|Domain|String|domain|域名

 |
|ExpiredTime|String|1544411108000|付费到期时间

 |
|OrganizationCount|Integer|2|组织数

 |
|OwnerBid|String|26842|创建者业务ID

 |
|OwnerName|String|uid-125566|创建者

 |
|OwnerUid|Integer|12042815|创建者用户ID

 |
|RegionId|String|cn-hangzhou|地域

 |
|RequestId|String|3A929FAC-A82D-4EAB-A0FF-D867426D8B23|请求ID

 |
|SpecName|String|basic|联盟节点规格

 |
|State|String|Pending|状态

 |
|SupportChannelConfig|Boolean|true|是否支持自定义配置参数

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricConsortiums
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricConsortiumsResponse>
  <Result>
		    <Domain>perf9141perf9141perf9141pef9141.asdadadewdasada.top</Domain>
		    <ConsortiumId>10000</ConsortiumId>
		    <OrganizationCount>2</OrganizationCount>
		    <ChannelCount>0</ChannelCount>
		    <ConsortiumName>quickstart</ConsortiumName>
		    <DeleteTime></DeleteTime>
		    <OwnerUid>1204281570282129</OwnerUid>
		    <State>Created</State>
		    <RegionId>cn-beijing</RegionId>
		    <RequestId>3A929FAC-A82D-4EAB-A0FF-D867426D8B23</RequestId>
		    <CreateTime>2018-07-16T05:31:32.000+0000</CreateTime>
		    <CodeName>quickstart</CodeName>
		    <OwnerName>uid-1204281570282129</OwnerName>
		    <OwnerBid>26842</OwnerBid>
		    <ChannelPolicy>Any</ChannelPolicy>
		    <SpecName>basic</SpecName>
		    <SupportChannelConfig>true</SupportChannelConfig>
	  </Result>
	  <RequestId>C445762C-8909-4BD8-A2BD-BB45BF2441D8</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricConsortiumsResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"ConsortiumName":"quickstart",
			"Domain":"perf9141perf9141perf9141pef9141.asdadadewdasada.top",
			"ConsortiumId":"10000",
			"OrganizationCount":2,
			"OwnerBid":"26842",
			"ChannelCount":0,
			"DeleteTime":"",
			"OwnerUid":1204281570282129,
			"SpecName":"basic",
			"State":"Created",
			"SupportChannelConfig":true,
			"RegionId":"cn-beijing",
			"RequestId":"3A929FAC-A82D-4EAB-A0FF-D867426D8B23",
			"CreateTime":"2018-07-16T05:31:32.000+0000",
			"CodeName":"quickstart",
			"ChannelPolicy":"Any",
			"OwnerName":"uid-1204281570282129"
		}
	],
	"RequestId":"C445762C-8909-4BD8-A2BD-BB45BF2441D8",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

