# CreateFabricChannelMember {#doc_api_Baas_CreateFabricChannelMember .reference}

调用CreateFabricChannelMember将其他组织添加到通道中。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CreateFabricChannelMember&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ChannelId|String|是|chan-channelx-1l1hmckuuisxo|通道ID

 |
|Action|String|否|CreateFabricChannelMember|系统规定参数。取值：**CreateFabricChannelMember**。

 |
|Organization.N.OrganizationId|String|否|peers-aaaaaa1-1oxw31d046jtl|组织ID

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
|Result|Boolean|true|结果

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CreateFabricChannelMember
&ChannelId=chan-channelx-1l1hmckuuisxo
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<CreateFabricChannelMemberResponse>
	  <Result>true</Result>
	  <RequestId>1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</CreateFabricChannelMemberResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":true,
	"RequestId":"1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

