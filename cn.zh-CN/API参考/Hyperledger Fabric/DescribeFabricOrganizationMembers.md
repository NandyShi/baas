# DescribeFabricOrganizationMembers {#doc_api_Baas_DescribeFabricOrganizationMembers .reference}

调用DescribeFabricOrganizationMembers获取该组织所加入的联盟与联盟成员。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricOrganizationMembers&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricOrganizationMembers|系统规定参数。取值：**DescribeFabricOrganizationMembers**。

 |
|OrganizationId|String|是|peers-aaaaaa2-1eqnj5o5w\*\*\*\*|组织ID

 |
|Location|String|否|cn-hangzhou|位置信息

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
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwl\*\*\*\*|联盟ID

 |
|ConsortiumName|String|name|联盟名称

 |
|Description|String|desc|描述

 |
|Domain|String|domain|域名

 |
|JoinedTime|String|1533025590|加入联盟的时间

 |
|OrganizationId|String|peers-aaaaaa2-1eqnj5o5w\*\*\*\*|组织ID

 |
|OrganizationName|String|name|组织名

 |
|State|String|Running|状态

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricOrganizationMembers
&OrganizationId=peers-aaaaaa2-1eqnj5o5w****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricOrganizationMembersResponse>
	  <Result>
		    <OrganizationId>consortium-xxxxxx</OrganizationId>
		    <OrganizationName>orgname</OrganizationName>
		    <JoinedTime>1533025590</JoinedTime>
		    <ConsortiumName>联盟</ConsortiumName>
		    <Description></Description>
		    <Domain>zhuangbsdadadadasdASdaefility.abasssample.cc</Domain>
		    <State>Approved</State>
		    <ConsortiumId>consortium-avengers-jkdhdif89****</ConsortiumId>
	  </Result>
	  <RequestId>C445762C-8909-4BD8-A2BD-BB45BF2441D8</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricOrganizationMembersResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"ConsortiumName":"联盟",
		"Description":"",
		"ConsortiumId":"consortium-avengers-jkdhdif89****",
		"State":"Approved",
		"Domain":"zhuangbsdadadadasdASdaefility.abasssample.cc",
		"JoinedTime":"1533025590",
		"OrganizationId":"consortium-xxxxxx",
		"OrganizationName":"orgname"
	},
	"RequestId":"C445762C-8909-4BD8-A2BD-BB45BF2441D8",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

