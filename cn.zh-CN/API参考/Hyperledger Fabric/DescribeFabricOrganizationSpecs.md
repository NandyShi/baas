# DescribeFabricOrganizationSpecs {#doc_api_Baas_DescribeFabricOrganizationSpecs .reference}

调用DescribeFabricOrganizationSpecs查询组织的规格列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricOrganizationSpecs&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricOrganizationSpecs|系统规定参数。取值：**DescribeFabricOrganizationSpecs**。

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
|Result| | |组织的规格列表

 |
|Enable|Boolean|true|是否启用

 |
|OrganizationSpecsName|String|basic|规格名

 |
|Title|String|基础版|标题

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricOrganizationSpecs
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricOrganizationSpecsResponse>
	  <Result>
		    <OrganizationSpecsName>basic</OrganizationSpecsName>
		    <Enable>true</Enable>
		    <Title>基础版</Title>
	  </Result>
	  <Result>
		    <OrganizationSpecsName>enterprise</OrganizationSpecsName>
		    <Enable>false</Enable>
		    <Title>企业版</Title>
	  </Result>
	  <RequestId>D44A00CF-95E0-48D9-A831-716E791D423E</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricOrganizationSpecsResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"OrganizationSpecsName":"basic",
			"Enable":true,
			"Title":"基础版"
		},
		{
			"OrganizationSpecsName":"enterprise",
			"Enable":false,
			"Title":"企业版"
		}
	],
	"RequestId":"D44A00CF-95E0-48D9-A831-716E791D423E",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

