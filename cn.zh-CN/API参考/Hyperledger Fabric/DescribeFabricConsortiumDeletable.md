# DescribeFabricConsortiumDeletable {#doc_api_Baas_DescribeFabricConsortiumDeletable .reference}

调用DescribeFabricConsortiumDeletable查询联盟是否可删除。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricConsortiumDeletable&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ConsortiumId|String|是|consortium-lianmenyumingyi-hc5d1bwl\*\*\*\*|联盟ID

 |
|Action|String|否|DescribeFabricConsortiumDeletable|系统规定参数。取值：**DescribeFabricConsortiumDeletable**。

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
|CodeName|String|codename|域名前缀

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

 |
|ConsortiumName|String|myconsortium|联盟名

 |
|Deletable|Boolean|true|是否可删除

 |
|Description|String|description|描述

 |
|Domain|String|domain|域名

 |
|RegionId|String|cn-hangzhou|地域

 |
|State|String|Running|状态

 |
|ZoneId|String|cn-hangzhou|可用区

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricConsortiumDeletable
&ConsortiumId=consortium-lianmenyumingyi-hc5d1bwl****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricConsortiumDeletableResponse>
	  <Result>
		    <ConsortiumId>consortium-xxxxxx</ConsortiumId>
		    <Deletable>false</Deletable>
		    <CodeName>name</CodeName>
		    <Description>desc</Description>
		    <Domain>domain</Domain>
		    <Name>asset_mgmtv1.0.out</Name>
		    <State>Checking</State>
		    <RegionId>cn-hangzhou</RegionId>
		    <ZoneId>cn-hangzhou</ZoneId>
	  </Result>
	  <RequestId>C445762C-8909-4BD8-A2BD-BB45BF2441D8</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricConsortiumDeletableResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"Name":"asset_mgmtv1.0.out",
		"Description":"desc",
		"State":"Checking",
		"Domain":"domain",
		"ConsortiumId":"consortium-xxxxxx",
		"RegionId":"cn-hangzhou",
		"CodeName":"name",
		"ZoneId":"cn-hangzhou",
		"Deletable":false
	},
	"RequestId":"C445762C-8909-4BD8-A2BD-BB45BF2441D8",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

