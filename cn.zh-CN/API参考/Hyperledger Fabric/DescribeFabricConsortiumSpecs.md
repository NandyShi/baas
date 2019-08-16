# DescribeFabricConsortiumSpecs {#doc_api_Baas_DescribeFabricConsortiumSpecs .reference}

调用DescribeFabricConsortiumSpecs查询联盟的规格列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricConsortiumSpecs&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricConsortiumSpecs|系统规定参数。取值：**DescribeFabricConsortiumSpecs**。

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
|Result| | |联盟的规格列表

 |
|Enable|Boolean|true|是否启用

 |
|SpecName|String|basic|规格名

 |
|SpecTitle|String|基础版|标题

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricConsortiumSpecs
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricConsortiumSpecsResponse>
	  <Result>
		    <Name>basic</Name>
		    <NumOfNodes>3</NumOfNodes>
		    <WorkerDescription>4 Woker (4C8G 系统盘 100G SSD 云盘)</WorkerDescription>
		    <Enable>true</Enable>
		    <MasterDescription>3 Master (4C8G)</MasterDescription>
		    <Title>基础版</Title>
	  </Result>
	  <Result>
		    <Name>enterprise</Name>
		    <NumOfNodes>3</NumOfNodes>
		    <WorkerDescription>6 Woker (8C16G 系统盘 100G SSD 云盘)</WorkerDescription>
		    <Enable>false</Enable>
		    <MasterDescription>3 Master (4C8G)</MasterDescription>
		    <Title>企业版</Title>
	  </Result>
	  <Result>
		    <Name>enterprise-sgx</Name>
		    <NumOfNodes>3</NumOfNodes>
		    <WorkerDescription>4 Woker (神龙 SGX 8C32G 系统盘 100G SSD 云盘)</WorkerDescription>
		    <Enable>false</Enable>
		    <MasterDescription>3 Master (4C8G)</MasterDescription>
		    <Title>企业安全版</Title>
	  </Result>
	  <RequestId>00984305-408B-4499-9822-5B720D96B381</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricConsortiumSpecsResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"Name":"basic",
			"WorkerDescription":"4 Woker (4C8G 系统盘 100G SSD 云盘)",
			"NumOfNodes":3,
			"Enable":true,
			"MasterDescription":"3 Master (4C8G)",
			"Title":"基础版"
		},
		{
			"Name":"enterprise",
			"WorkerDescription":"6 Woker (8C16G 系统盘 100G SSD 云盘)",
			"NumOfNodes":3,
			"Enable":false,
			"MasterDescription":"3 Master (4C8G)",
			"Title":"企业版"
		},
		{
			"Name":"enterprise-sgx",
			"WorkerDescription":"4 Woker (神龙 SGX 8C32G 系统盘 100G SSD 云盘)",
			"NumOfNodes":3,
			"Enable":false,
			"MasterDescription":"3 Master (4C8G)",
			"Title":"企业安全版"
		}
	],
	"RequestId":"00984305-408B-4499-9822-5B720D96B381",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

