# DeleteAntChainConsortium {#doc_api_Baas_DeleteAntChainConsortium .reference}

删除联盟

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DeleteAntChainConsortium&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ConsortiumId|String|是|q0oWq92P|联盟ID

 |
|Action|String|否|DeleteAntChainConsortium|系统规定参数。取值：DeleteAntChainConsortium。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|F3685787-9F2F-4D60-ADD6-07A5179552CA|请求ID

 |
|Result|String|success|请求结果

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DeleteAntChainConsortium
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<xml version="1.0" encoding="UTF-8">
	  <code>200</code>
	  <data>
		    <RequestId>F3685787-9F2F-4D60-ADD6-07A5179552CA</RequestId>
		    <Result>success</Result>
	  </data>
	  <requestId>F3685787-9F2F-4D60-ADD6-07A5179552CA</requestId>
	  <successResponse>true</successResponse>
</xml>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"F3685787-9F2F-4D60-ADD6-07A5179552CA",
	"data":{
		"Result":"success",
		"RequestId":"F3685787-9F2F-4D60-ADD6-07A5179552CA"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

