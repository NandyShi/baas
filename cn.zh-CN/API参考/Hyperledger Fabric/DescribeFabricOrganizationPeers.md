# DescribeFabricOrganizationPeers {#doc_api_Baas_DescribeFabricOrganizationPeers .reference}

调用DescribeFabricOrganizationPeers获取组织的节点列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricOrganizationPeers&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricOrganizationPeers|系统规定参数。取值：**DescribeFabricOrganizationPeers**。

 |
|OrganizationId|String|是|peers-aaaaaa2-1eqnj5o5w\*\*\*\*|组织ID

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
|Result| | |组织的节点列表

 |
|CreateTime|String|1533025590|创建时间

 |
|Domain|String|domain|域名

 |
|InstanceType|String|basic|实例类型

 |
|InternetIp|String|10.0.0.2|公网IP

 |
|IntranetIp|String|10.0.0.2|内网IP

 |
|IsAnchor|Boolean|false|是否是AnchorPeer

 |
|OrganizationPeerName|String|name|组织的节点名

 |
|Port|Integer|1234|端口

 |
|UpdateTime|String|1533025590|更新时间

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricOrganizationPeers
&OrganizationId=peers-aaaaaa2-1eqnj5o5w****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricOrganizationPeersResponse>
	  <Result>
		    <Port>7050</Port>
		    <Domain>peer1.taosafddasffsadfasaddsadbao.aliyunbaas.top</Domain>
		    <IsAnchor>true</IsAnchor>
		    <CreateTime>2018-07-01 09:00:00</CreateTime>
		    <UpdateTime>2018-07-02 09:00:00</UpdateTime>
		    <InternetIp>8.8.8.1</InternetIp>
		    <InstanceType>ecs.n1.small</InstanceType>
		    <IntranetIp>8.8.8.1</IntranetIp>
		    <OrganizationPeerName>name</OrganizationPeerName>
	  </Result>
	  <RequestId>C445762C-8909-4BD8-A2BD-BB45BF2441D8</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricOrganizationPeersResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"Port":7050,
		"OrganizationPeerName":"name",
		"IsAnchor":true,
		"Domain":"peer1.taosafddasffsadfasaddsadbao.aliyunbaas.top",
		"IntranetIp":"8.8.8.1",
		"CreateTime":"2018-07-01 09:00:00",
		"InternetIp":"8.8.8.1",
		"UpdateTime":"2018-07-02 09:00:00",
		"InstanceType":"ecs.n1.small"
	},
	"RequestId":"C445762C-8909-4BD8-A2BD-BB45BF2441D8",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

