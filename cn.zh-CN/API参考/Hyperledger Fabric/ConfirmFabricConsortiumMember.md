# ConfirmFabricConsortiumMember {#doc_api_Baas_ConfirmFabricConsortiumMember .reference}

调用ConfirmFabricConsortiumMember确认联盟成员的加入申请，需要确认提案。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=ConfirmFabricConsortiumMember&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|ConfirmFabricConsortiumMember|系统规定参数。取值：**ConfirmFabricConsortiumMember**。

 |
|ConsortiumId|String|是|consortium-aaaaaa-akpcsjjac2jd|联盟ID。

 |
|Organization.N.OrganizationId|String|否|peers-aaaaaa1-1oxw31d046jtl|组织的ID列表。

 |
|RegionId|String|否|cn-hangzhou|地域。

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|ErrorCode|Integer|200|错误码

 |
|RequestId|String|50B3ACF3-CE12-433C-A834-9E8C657A4934|请求ID

 |
|Result|Boolean|true|结果

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=ConfirmFabricConsortiumMember
&ConsortiumId=consortium-aaaaaa-akpcsjjac2jd
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<ConfirmFabricConsortiumMemberResponse>
	  <Result>true</Result>
	  <RequestId>39444730-DCF6-453E-931C-C6294F9CB187</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</ConfirmFabricConsortiumMemberResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":"true",
	"RequestId":"39444730-DCF6-453E-931C-C6294F9CB187",
	"ErrorCode":"200",
	"Success":"true"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

