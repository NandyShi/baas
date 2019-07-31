# DescribeFabricChaincodeUploadPolicy {#doc_api_Baas_DescribeFabricChaincodeUploadPolicy .reference}

调用DescribeFabricChaincodeUploadPolicy获取上传链码策略。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricChaincodeUploadPolicy&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|OrganizationId|String|是|peers-aaaaaa1-1oxw31d04\*\*\*\*|组织ID

 |
|Action|String|否|DescribeFabricChaincodeUploadPolicy|系统规定参数。取值：**DescribeFabricChaincodeUploadPolicy**。

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
|Result| | |结果

 |
|AccessId|String|accessId|访问OSS的ID

 |
|Dir|String|test3/4bd1de21-2fff-4405-a8e9-f864c4bee24f|上传目录

 |
|Expire|Integer|1533025590|过期时间

 |
|Host|String|https://chaincode.oss-cn-beijing.aliyuncs.com|OSS域名

 |
|Policy|String|eyJleHBpcmF0aW9uIjoiMjAxOC0wNy0zMVQwODoyNjozMC40NzdaIiwiY29uZGl|OSS安全策略

 |
|Signature|String|signature|OSS签名

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricChaincodeUploadPolicy
&OrganizationId=peers-aaaaaa1-1oxw31d04****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricChaincodeUploadPolicyResponse>
	  <Result>
		    <Dir>t/4bd1de21-2fff-4</Dir>
		    <Host>https://oss.aliyuncs.com</Host>
		    <Policy>eyJleHBpcmF0aW9uIjoiMjAxOC0wNy0zMVQwODoyNjozMC40NzdaIiwiY29uZGl0aW9ucyI6W1siY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMTA0ODU3NjAwMF0sWyJzdGFydHMtd2l0aCIsIiRrZXkiLCJ0ZXN0My80YmQxZGUyMS0yZmZmLTQ0MDUtYThlOS1mODY0YzRiZWUyNGYiXV19</Policy>
		    <Expire>1533025590</Expire>
		    <AccessId>accessId</AccessId>
		    <Signature>klI/signature=</Signature>
	  </Result>
	  <RequestId>540BFE13-BDE5-40B9-BCDD-F2E24B6D064F</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricChaincodeUploadPolicyResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"Dir":"t/4bd1de21-2fff-4",
		"Host":"https://oss.aliyuncs.com",
		"Policy":"eyJleHBpcmF0aW9uIjoiMjAxOC0wNy0zMVQwODoyNjozMC40NzdaIiwiY29uZGl0aW9ucyI6W1siY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMTA0ODU3NjAwMF0sWyJzdGFydHMtd2l0aCIsIiRrZXkiLCJ0ZXN0My80YmQxZGUyMS0yZmZmLTQ0MDUtYThlOS1mODY0YzRiZWUyNGYiXV19",
		"Expire":1533025590,
		"AccessId":"accessId",
		"Signature":"klI/signature="
	},
	"RequestId":"540BFE13-BDE5-40B9-BCDD-F2E24B6D064F",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

