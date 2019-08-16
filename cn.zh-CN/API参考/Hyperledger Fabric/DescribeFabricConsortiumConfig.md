# DescribeFabricConsortiumConfig {#doc_api_Baas_DescribeFabricConsortiumConfig .reference}

调用DescribeFabricConsortiumConfig获取“创建联盟”的参数可选值。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricConsortiumConfig&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricConsortiumConfig|系统规定参数。取值：**DescribeFabricConsortiumConfig**。

 |
|RegionId|String|否|cn-hangzhou|地域。

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|ErrorCode|Integer|200|错误码。

 |
|RequestId|String|1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3|请求ID。

 |
|Result| | |“创建联盟”的参数可选值。

 |
|ChannelPolicy| |\[ "Any" \]|创建通道策略。

 |
|OrdererType| |\[ "Solo", "Kafka" \]|Orderer类型。

 |
|Success|Boolean|true|是否成功。

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricConsortiumConfig
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricConsortiumConfigResponse>
	  <Result>
		    <OrdererType>Solo</OrdererType>
		    <OrdererType>Kafka</OrdererType>
		    <ChannelPolicy>Any</ChannelPolicy>
	  </Result>
	  <RequestId>1D606B42-57BD-486E-8CAB-E184A1C37E57</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricConsortiumConfigResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"OrdererType":[
			"Solo",
			"Kafka"
		],
		"ChannelPolicy":[
			"Any"
		]
	},
	"RequestId":"1D606B42-57BD-486E-8CAB-E184A1C37E57",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

