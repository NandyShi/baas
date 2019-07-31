# DescribeFabricCandidateOrganizations {#doc_api_Baas_DescribeFabricCandidateOrganizations .reference}

调用DescribeFabricCandidateOrganizations查询接收邀请的候选组织。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricCandidateOrganizations&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|否|DescribeFabricCandidateOrganizations|系统规定参数。取值：**DescribeFabricCandidateOrganizations**。

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
|ClusterState|String|Running|集群状态

 |
|OrganizationId|String|peers-1oxw31d04\*\*\*\*|组织ID

 |
|OrganizationName|String|org1|组织名

 |
|ServiceState|String|Running|服务状态

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricCandidateOrganizations
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricCandidateOrganizationsResponse>
	  <Result>
		    <ClusterState>Serving</ClusterState>
		    <OrganizationId>org-3hke7gfkjh****</OrganizationId>
		    <ServiceState>Created</ServiceState>
		    <OrganizationName>blockchain_ruiqi_test</OrganizationName>
	  </Result>
	  <Result>
		    <ClusterState>Serving</ClusterState>
		    <OrganizationId>org-2nba94f601****</OrganizationId>
		    <ServiceState>Failed</ServiceState>
		    <OrganizationName>test</OrganizationName>
	  </Result>
	  <RequestId>1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricCandidateOrganizationsResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"ClusterState":"Serving",
			"OrganizationId":"org-3hke7gfkjh****",
			"ServiceState":"Created",
			"OrganizationName":"blockchain_ruiqi_test"
		},
		{
			"ClusterState":"Serving",
			"OrganizationId":"org-2nba94f601****",
			"ServiceState":"Failed",
			"OrganizationName":"test"
		}
	],
	"RequestId":"1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

