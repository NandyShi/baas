# DescribeFabricOrganizations {#doc_api_Baas_DescribeFabricOrganizations .reference}

调用DescribeFabricOrganizations获取组织列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricOrganizations&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricOrganizations|系统规定参数。取值：**DescribeFabricOrganizations**。

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
|Result| | |组织列表

 |
|CodeName|String|name|域名前缀

 |
|ConsortiumCount|Integer|2|联盟数量

 |
|CreateTime|String|1533025590|创建时间

 |
|Domain|String|domain|域名

 |
|OrganizationDescription|String|desc|组织描述

 |
|OrganizationId|String|peers-aaaaaa2-1eqnj5o5w9dt3|组织ID

 |
|OrganizationName|String|name|组织名

 |
|OwnerBid|String|bid|创建者业务ID

 |
|OwnerName|String|name|创建者

 |
|OwnerUid|Integer|1232|创建者用户ID

 |
|PeerCount|Integer|3|节点数

 |
|RegionId|String|cn-hangzhou|地域

 |
|RequestId|String|1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3|请求ID

 |
|SpecName|String|basic、|规格名

 |
|State|String|Running|状态

 |
|UserCount|Integer|10|用户数量

 |
|ZoneId|String|zone|可用区

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricOrganizations
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricOrganizationsResponse>
  <Result>
		    <OrganizationDescription>perf9141pe rf9141perf 9141perf9 141perf9141perf9141perf9 141pe rf9141perf91 41perf914 1perf9141perf 9141perf9141perf9141perf9141</OrganizationDescription>
		    <Domain>perf9141perf9adsadasdasdasdadaasd141perf9141pef9141.abasssample.cc</Domain>
		    <ZoneId>cn-shanghai-a</ZoneId>
		    <OrganizationId>org-perf9141-7digc71bg</OrganizationId>
		    <OrganizationName>organization ConsortiumId ConsortiumId ads ConsortiumId sdaConsortiumId</OrganizationName>
		    <ConsortiumCount>0</ConsortiumCount>
		    <UserCount>0</UserCount>
		    <SpecName>ecs.n1.medium</SpecName>
		    <State>Created</State>
		    <RegionId>cn-shanghai</RegionId>
		    <RequestId>BEB5EB54-414E-4EF9-8C8A-F1AE2EF7BA2D</RequestId>
		    <CreateTime>2018-07-02T08:22:26.000+0000</CreateTime>
		    <CodeName>perf9141</CodeName>
		    <PeerCount>2</PeerCount>
  </Result>
  <RequestId>7D27692E-C501-4B1D-878C-0B869DD3D9E6</RequestId>
  <Success>true</Success>
  <ErrorCode>200</ErrorCode>
</DescribeFabricOrganizationsResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"Domain":"perf9141perf9adsadasdasdasdadaasd141perf9141pef9141.abasssample.cc",
		"ZoneId":"cn-shanghai-a",
		"OrganizationId":"org-perf9141-7digc71bg",
		"OrganizationName":"organization ConsortiumId ConsortiumId ads ConsortiumId sdaConsortiumId",
		"OrganizationDescription":"perf9141pe rf9141perf 9141perf9 141perf9141perf9141perf9 141pe rf9141perf91 41perf914 1perf9141perf 9141perf9141perf9141perf9141",
		"ConsortiumCount":0,
		"UserCount":0,
		"SpecName":"ecs.n1.medium",
		"State":"Created",
		"RegionId":"cn-shanghai",
		"RequestId":"BEB5EB54-414E-4EF9-8C8A-F1AE2EF7BA2D",
		"CreateTime":"2018-07-02T08:22:26.000+0000",
		"CodeName":"perf9141",
		"PeerCount":2
	},
	"RequestId":"7D27692E-C501-4B1D-878C-0B869DD3D9E6",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

