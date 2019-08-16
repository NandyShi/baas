# CreateFabricChaincode {#doc_api_Baas_CreateFabricChaincode .reference}

调用CreateFabricChaincode创建链码。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=CreateFabricChaincode&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|CreateFabricChaincode|系统规定参数。取值：**CreateFabricChaincode**。

 |
|ChannelId|String|是|chan-first-channel-1w55v3u39x2xz|通道ID

 |
|ConsortiumId|String|是|consortium-aaaaaa-akpcsjjac2jd|联盟ID

 |
|OrganizationId|String|是|peers-aaaaaa1-1oxw31d046jtl|组织ID

 |
|OssBucket|String|是|https://chaincode.oss-cn-beijing.aliyuncs.com|Oss桶地址

 |
|OssUrl|String|是|aaaaaa1/a0cf8729-7d47-44c9-9ed5-6d2fdfc8dc2c/sacc.cc|Oss对象地址

 |
|EndorsePolicy|String|否|OR \('aaaaaa1MSP.peer'\)|背书策略

 |
|Location|String|否|cn-hangzhou|位置信息

 |
|RegionId|String|否|cn-hangzhou|地域

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|ErrorCode|Integer|200|错误码

 |
|RequestId|String|CD264CC8-B892-4CDC-BD31-7D179EE6E396|请求ID

 |
|Result| | |创建结果

 |
|ChaincodeId|String|code-sacc-1pr09q7jmo0np|链码ID

 |
|ChaincodeName|String|mychaincode|链码名

 |
|ChaincodeVersion|String|1.0|链码版本

 |
|ChannelName|String|first-channel|通道名

 |
|ConsortiumId|String|consortium-aaaaaa-akpcsjjac2jd|联盟ID

 |
|CreateTime|String|1544766801000|创建时间

 |
|DeployTime|String|1544766801000|部署时间

 |
|EndorsePolicy|String|OR \('aaaaaa1MSP.peer'\)|背书策略

 |
|Input|String|string|输入

 |
|Install|Boolean|true|是否安装

 |
|Message|String|string|消息

 |
|Path|String|go-sdk-demo/chaincode/src|路径

 |
|ProviderId|String|peers-aaaaaa1-1oxw31d046jtl|上传ID

 |
|ProviderName|String|peers-aaaaaa1-1oxw31d046jtl|上传者名字

 |
|State|String|Instantiatable|状态

 |
|Type|Integer|1|类型

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CreateFabricChaincode
&ChannelId=chan-first-channel-1w55v3u39x2xz
&ConsortiumId=consortium-aaaaaa-akpcsjjac2jd
&OrganizationId=peers-aaaaaa1-1oxw31d046jtl
&OssBucket=https://chaincode.oss-cn-beijing.aliyuncs.com
&OssUrl=aaaaaa1/a0cf8729-7d47-44c9-9ed5-6d2fdfc8dc2c/sacc.cc
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<CreateFabricChaincodeResponse>
	  <Result>
		    <ChaincodeName>sacc</ChaincodeName>
		    <ChannelId>chan-first-channel-1w55v3u39x2xz</ChannelId>
		    <State>Instantiatable</State>
		    <ConsortiumId>consortium-aaaaaa-akpcsjjac2jd</ConsortiumId>
		    <Creator>aaaaaa1</Creator>
		    <CreateTime>1544766801000</CreateTime>
		    <Install>true</Install>
		    <ChannelName>first-channel</ChannelName>
		    <ChaincodeVersion>1.0</ChaincodeVersion>
		    <EndorsePolicy>OR (&amp;#39;aaaaaa1MSP.peer&amp;#39;)</EndorsePolicy>
		    <ChaincodeId>code-sacc-1pr09q7jmo0np</ChaincodeId>
	  </Result>
	  <RequestId>50B3ACF3-CE12-433C-A834-9E8C657A4934</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</CreateFabricChaincodeResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"ChannelId":"chan-first-channel-1w55v3u39x2xz",
			"ChaincodeVersion":"1.0",
			"Install":"true",
			"ConsortiumId":"consortium-aaaaaa-akpcsjjac2jd",
			"State":"Instantiatable",
			"ChaincodeName":"sacc",
			"Creator":"aaaaaa1",
			"CreateTime":1544766801000,
			"ChannelName":"first-channel",
			"EndorsePolicy":"OR (&#39;aaaaaa1MSP.peer&#39;)",
			"ChaincodeId":"code-sacc-1pr09q7jmo0np"
		}
	],
	"RequestId":"50B3ACF3-CE12-433C-A834-9E8C657A4934",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

|HttpCode|错误码|错误信息|描述|
|--------|---|----|--|
|400|ChaincodeDuplicated|The chaincode \[%s\] of version \[%s\] already exists, please change the name or the version of the chaincode.|已经存在链码\[%s\]版本是\[%s\]，请修改链码名称或者版本|
|400|ChaincodeInvalid|The format of the chaincode package is invalid.|链码格式错误|

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

