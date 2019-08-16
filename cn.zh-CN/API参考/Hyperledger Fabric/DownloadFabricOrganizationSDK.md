# DownloadFabricOrganizationSDK {#doc_api_Baas_DownloadFabricOrganizationSDK .reference}

调用DownloadFabricOrganizationSDK下载SDK。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DownloadFabricOrganizationSDK&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DownloadFabricOrganizationSDK|系统规定参数。取值：**DownloadFabricOrganizationSDK**。

 |
|OrganizationId|String|是|peers-aaaaaa2-1eqnj5o5w\*\*\*\*|组织ID

 |
|Username|String|是|username|用户名

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
|Result| | |结果

 |
|Content|String|base64string|base64转码过的文件内容，需要用base64解码才能得到文件原内容。

 |
|Path|String|dir/file|文件解压后的路径

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DownloadFabricOrganizationSDK
&OrganizationId=peers-aaaaaa2-1eqnj5o5w****
&Username=username
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DownloadFabricOrganizationSDKResponse>
	  <Result>
		    <Content>base64string</Content>
		    <Path>dir/file</Path>
	  </Result>
	  <RequestId>7D27692E-C501-4B1D-878C-0B869DD3D9E6</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DownloadFabricOrganizationSDKResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"Content":"base64string",
		"Path":"dir/file"
	},
	"RequestId":"7D27692E-C501-4B1D-878C-0B869DD3D9E6",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

