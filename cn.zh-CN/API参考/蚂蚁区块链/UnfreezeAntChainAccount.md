# UnfreezeAntChainAccount {#doc_api_Baas_UnfreezeAntChainAccount .reference}

解冻一个蚂蚁区块链上的账户

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=UnfreezeAntChainAccount&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Account|String|是|accountname|账户名

 |
|AntChainId|String|是|1q8B5R9p|区块链ID

 |
|Action|String|否|UnfreezeAntChainAccount|系统规定参数。取值：UnfreezeAntChainAccount。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|6ED983D3-C131-4104-8BDD-1F37992258E1|请求ID

 |
|Result|String|success|请求结果

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=UnfreezeAntChainAccount
&Account=accountname
&AntChainId=1q8B5R9p
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<UnfreezeAntChainAccountResponse>
	  <code>200</code>
	  <data>
		    <RequestId>6ED983D3-C131-4104-8BDD-1F37992258E1</RequestId>
		    <Result>success</Result>
	  </data>
	  <requestId>6ED983D3-C131-4104-8BDD-1F37992258E1</requestId>
	  <successResponse>true</successResponse>
</UnfreezeAntChainAccountResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"6ED983D3-C131-4104-8BDD-1F37992258E1",
	"data":{
		"Result":"success",
		"RequestId":"6ED983D3-C131-4104-8BDD-1F37992258E1"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

