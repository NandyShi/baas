# DescribeFabricConsortiumMembers {#doc_api_Baas_DescribeFabricConsortiumMembers .reference}

调用DescribeFabricConsortiumMembers获取联盟的组织信息。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricConsortiumMembers&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricConsortiumMembers|系统规定参数。取值：**DescribeFabricConsortiumMembers**。

 |
|ConsortiumId|String|是|consortium-lianmenyumingyi-hc5d1bwl\*\*\*\*|联盟ID

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
|Result| | |联盟的组织信息

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

 |
|Description|String|description|描述

 |
|Domain|String|domain|域名

 |
|JoinedTime|String|1544411108000|加入联盟的时间

 |
|OrganizationId|String|peers-aaaaaa2-1eqnj5o5w9dt3|组织ID

 |
|OrganizationName|String|name|组织名

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricConsortiumMembers
&ConsortiumId=consortium-lianmenyumingyi-hc5d1bwl****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricConsortiumMembersResponse>
	  <Result>
		    <OrganizationName>测试3</OrganizationName>
		    <Description>测试3</Description>
		    <Domain>test3asdasdafreqweqwdsafsdfw3easda.abasssample.cc</Domain>
		    <JoinedTime>2018-07-31T08:08:01.000+0000</JoinedTime>
		    <ConsortiumId>consortium-testthree-3i6j6d8ian5668</ConsortiumId>
		    <OrganizationId>peers-test3-25c96n9n6jh3dc</OrganizationId>
	  </Result>
	  <RequestId>98B37CF5-AB0C-423E-8335-81A54899577E</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricConsortiumMembersResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"Description":"测试3",
			"ConsortiumId":"consortium-testthree-3i6j6d8ian5668",
			"JoinedTime":"2018-07-31T08:08:01.000+0000",
			"Domain":"test3asdasdafreqweqwdsafsdfw3easda.abasssample.cc",
			"OrganizationId":"peers-test3-25c96n9n6jh3dc",
			"OrganizationName":"测试3"
		}
	],
	"RequestId":"98B37CF5-AB0C-423E-8335-81A54899577E",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

