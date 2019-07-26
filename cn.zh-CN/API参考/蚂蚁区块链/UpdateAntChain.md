# UpdateAntChain {#doc_api_Baas_UpdateAntChain .reference}

更新一条蚂蚁区块链名字

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=UpdateAntChain&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|pYogqb9v|区块链ID

 |
|AntChainName|String|是|修改名称|区块链名称

 |
|Action|String|否|UpdateAntChain|系统规定参数。取值：UpdateAntChain。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|F6A52E53-2CCB-4C3C-A44D-45FAEBC24E47|请求ID

 |
|Result|String|success|请求结果

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=UpdateAntChain
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"F6A52E53-2CCB-4C3C-A44D-45FAEBC24E47",
	"data":{
		"Result":"success",
		"RequestId":"F6A52E53-2CCB-4C3C-A44D-45FAEBC24E47"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

