# CheckFabricConsortiumDomain {#doc_api_Baas_CheckFabricConsortiumDomain .reference}

调用CheckFabricConsortiumDomain检查联盟域名是否可用。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CheckFabricConsortiumDomain&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|DomainCode|String|是|bank|联盟域名。

 |
|Action|String|否|CheckFabricConsortiumDomain|系统规定参数。取值：**CheckFabricConsortiumDomain**。

 |
|RegionId|String|否|cn-hangzhou|地域。

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|ErrorCode|Integer|200|错误码

 |
|RequestId|String|8F80A214-89FC-4348-9B3F-15446B3DC1FA|请求ID

 |
|Result| | |处理结果

 |
|Domain|String|bank|域名

 |
|Prompt|String|OK|提示

 |
|Valid|Boolean|true|是否合法

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CheckFabricConsortiumDomain
&DomainCode=bank
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<CheckFabricConsortiumDomainResponse>
      <Result>
		    <Prompt>OK</Prompt>
		    <Domain>bank</Domain>
		    <Valid>true</Valid>
	  </Result>
	  <RequestId>8F80A214-89FC-4348-9B3F-15446B3DC1FA</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</CheckFabricConsortiumDomainResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"Prompt":"OK",
		"Domain":"bank",
		"Valid":true
	},
	"RequestId":"8F80A214-89FC-4348-9B3F-15446B3DC1FA",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

