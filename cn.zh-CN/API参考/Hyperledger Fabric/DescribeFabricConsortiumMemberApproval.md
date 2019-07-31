# DescribeFabricConsortiumMemberApproval {#doc_api_Baas_DescribeFabricConsortiumMemberApproval .reference}

调用DescribeFabricConsortiumMemberApproval获取联盟成员的审批状态列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricConsortiumMemberApproval&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ConsortiumId|String|是|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

 |
|Action|String|否|DescribeFabricConsortiumMemberApproval|系统规定参数。取值：**DescribeFabricConsortiumMemberApproval**。

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
|Result| | |联盟成员的审批状态列表

 |
|ChannelCreatePolicy|String|Any|通道创建策略

 |
|ConfirmTime|String|1544411108000|确认时间

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

 |
|ConsortiumName|String|name|联盟名

 |
|DomainName|String|domain|域名

 |
|OrganizationId|String|peers-aaaaaa2-1eqnj5o5w9dt3|组织ID

 |
|OrganizationName|String|orgname|组织名

 |
|State|String|Running|状态

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricConsortiumMemberApproval
&ConsortiumId=consortium-lianmenyumingyi-hc5d1bwlulg7
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricConsortiumMemberApprovalResponse>
	  <Result>
		    <ConfirmTime>1544411108000</ConfirmTime>
		    <ConsortiumName>阿里</ConsortiumName>
		    <State>Accepted</State>
		    <ConsortiumId>10000</ConsortiumId>
		    <DomainName>peer.apple.aliyunbaas.top</DomainName>
		    <ChannelCreatePolicy>1000</ChannelCreatePolicy>
		    <OrganizationId>1</OrganizationId>
		    <OrganizationName>苹果公司</OrganizationName>
	  </Result>
	  <Result>
		    <ConfirmTime>1544411108000</ConfirmTime>
		    <ConsortiumName>阿2里</ConsortiumName>
		    <State></State>
		    <ConsortiumId>10100</ConsortiumId>
		    <DomainName>peer.apple.aliyunbaas.top</DomainName>
		    <ChannelCreatePolicy>1000</ChannelCreatePolicy>
		    <OrganizationId>12</OrganizationId>
		    <OrganizationName>苹果公司</OrganizationName>
	  </Result>
	  <RequestId>C445762C-8909-4BD8-A2BD-BB45BF2441D8</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricConsortiumMemberApprovalResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"ConsortiumName":"阿里",
			"ConsortiumId":"10000",
			"State":"Accepted",
			"DomainName":"peer.apple.aliyunbaas.top",
			"ConfirmTime":"1544411108000",
			"ChannelCreatePolicy":"1000",
			"OrganizationId":"1",
			"OrganizationName":"苹果公司"
		},
		{
			"ConsortiumName":"阿2里",
			"ConsortiumId":"10100",
			"State":"",
			"DomainName":"peer.apple.aliyunbaas.top",
			"ConfirmTime":"1544411108000",
			"ChannelCreatePolicy":"1000",
			"OrganizationId":"12",
			"OrganizationName":"苹果公司"
		}
	],
	"RequestId":"C445762C-8909-4BD8-A2BD-BB45BF2441D8",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

