# FreezeAntChainAccount {#doc_api_Baas_FreezeAntChainAccount .reference}

冻结一个蚂蚁区块链上的账户

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=FreezeAntChainAccount&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Account|String|是|accountname|账户名称

 |
|AntChainId|String|是|1q8B5R9p|区块链ID

 |
|Action|String|否|FreezeAntChainAccount|系统规定参数。取值：FreezeAntChainAccount。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|9F862442-F6AD-4B5F-8969-CE23DE1413CB|请求ID

 |
|Result|String|success|请求结果

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=FreezeAntChainAccount
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"9F862442-F6AD-4B5F-8969-CE23DE1413CB",
	"data":{
		"Result":"success",
		"RequestId":"9F862442-F6AD-4B5F-8969-CE23DE1413CB"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

