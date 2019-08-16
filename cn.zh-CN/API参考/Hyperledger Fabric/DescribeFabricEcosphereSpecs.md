# DescribeFabricEcosphereSpecs {#doc_api_Baas_DescribeFabricEcosphereSpecs .reference}

调用DescribeFabricEcosphereSpecs查询快速模式的规格列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricEcosphereSpecs&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricEcosphereSpecs|系统规定参数。取值：**DescribeFabricEcosphereSpecs**。

 |
|RegionId|String|否|cn-hangzhou|地域。

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|ErrorCode|Integer|200|错误码

 |
|RequestId|String|1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3|请求ID

 |
|Result| | |快速模式的规格列表

 |
|Enable|Boolean|true|是否可用

 |
|SpecName|String|enterprise|规格名称

 |
|SpecTitle|String|企业版|规格标题

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricEcosphereSpecs
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricEcosphereSpecsResponse>
	  <Result>
		    <SpecName>basic</SpecName>
		    <NumOfNodes>3</NumOfNodes>
		    <WorkerDescription>4 Woker (4C8G 系统盘 100G SSD 云盘)</WorkerDescription>
		    <Enable>true</Enable>
		    <MasterDescription>3 Master (4C8G)</MasterDescription>
		    <SpecTitle>基础版</SpecTitle>
	  </Result>
	  <Result>
		    <SpecName>enterprise</SpecName>
		    <NumOfNodes>3</NumOfNodes>
		    <WorkerDescription>6 Woker (8C16G 系统盘 100G SSD 云盘)</WorkerDescription>
		    <Enable>false</Enable>
		    <MasterDescription>3 Master (4C8G)</MasterDescription>
		    <SpecTitle>企业版</SpecTitle>
	  </Result>
	  <Result>
		    <SpecName>enterprise-sgx</SpecName>
		    <NumOfNodes>3</NumOfNodes>
		    <WorkerDescription>4 Woker (神龙 SGX 8C32G 系统盘 100G SSD 云盘)</WorkerDescription>
		    <Enable>false</Enable>
		    <MasterDescription>3 Master (4C8G)</MasterDescription>
		    <SpecTitle>企业安全版</SpecTitle>
	  </Result>
	  <RequestId>2537DB1B-F478-431E-A847-5DDAAE2BD251</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricEcosphereSpecsResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"WorkerDescription":"4 Woker (4C8G 系统盘 100G SSD 云盘)",
			"NumOfNodes":3,
			"SpecName":"basic",
			"Enable":true,
			"SpecTitle":"基础版",
			"MasterDescription":"3 Master (4C8G)"
		},
		{
			"WorkerDescription":"6 Woker (8C16G 系统盘 100G SSD 云盘)",
			"NumOfNodes":3,
			"SpecName":"enterprise",
			"Enable":false,
			"SpecTitle":"企业版",
			"MasterDescription":"3 Master (4C8G)"
		},
		{
			"WorkerDescription":"4 Woker (神龙 SGX 8C32G 系统盘 100G SSD 云盘)",
			"NumOfNodes":3,
			"SpecName":"enterprise-sgx",
			"Enable":false,
			"SpecTitle":"企业安全版",
			"MasterDescription":"3 Master (4C8G)"
		}
	],
	"RequestId":"2537DB1B-F478-431E-A847-5DDAAE2BD251",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

