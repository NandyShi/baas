# AcceptFabricInvitation {#doc_api_Baas_AcceptFabricInvitation .reference}

调用AcceptFabricInvitation接受加入联盟的邀请。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=AcceptFabricInvitation&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Code|String|是|secrettoken|邀请码。

 |
|Action|String|否|AcceptFabricInvitation|系统规定参数。取值：**AcceptFabricInvitation**。

 |
|IsAccepted|Boolean|否|true|是否接受。

 |
|RegionId|String|否|cn-hangzhou|地域。

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|ErrorCode|Integer|200|错误码

 |
|RequestId|String|52CC8D5B-79A8-4769-BC7B-8940556ADA49|请求ID

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=AcceptFabricInvitation
&Code=secrettoken
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<AcceptFabricInvitationResesponse>
	  <RequestId>52CC8D5B-79A8-4769-BC7B-8940556ADA49</RequestId>
	  <ErrorCode>200</ErrorCode>
	  <Success>true</Success>
</AcceptFabricInvitationResesponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"RequestId":"52CC8D5B-79A8-4769-BC7B-8940556ADA49",
	"Success":true,
	"ErrorCode":200
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

