# DescribeFabricConsortiumAdminStatus {#doc_api_Baas_DescribeFabricConsortiumAdminStatus .reference}

调用DescribeFabricConsortiumAdminStatus获取联盟管理状态信息。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricConsortiumAdminStatus&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|否|DescribeFabricConsortiumAdminStatus|系统规定参数。取值：**DescribeFabricConsortiumAdminStatus**。

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
|Result| | |联盟管理状态信息

 |
|ConsortiumAdministrator|Boolean|true|是否为盟主

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricConsortiumAdminStatus
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricConsortiumAdminStatusResponse>
	  <Result>
		    <ConsortiumId>10000</ConsortiumId>
		    <ConsortiumAdministrator>true</ConsortiumAdministrator>
	  </Result>
	  <Result>
		    <ConsortiumId>10001</ConsortiumId>
		    <ConsortiumAdministrator>false</ConsortiumAdministrator>
	  </Result>
	  <RequestId>3E85A941-658C-40E8-9704-60513A0281CF</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricConsortiumAdminStatusResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"ConsortiumId":"10000",
			"ConsortiumAdministrator":true
		},
		{
			"ConsortiumId":"10001",
			"ConsortiumAdministrator":false
		}
	],
	"RequestId":"3E85A941-658C-40E8-9704-60513A0281CF",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

