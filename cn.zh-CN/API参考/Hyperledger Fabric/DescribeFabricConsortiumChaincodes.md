# DescribeFabricConsortiumChaincodes {#doc_api_Baas_DescribeFabricConsortiumChaincodes .reference}

调用DescribeFabricConsortiumChaincodes获取联盟的链码列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricConsortiumChaincodes&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricConsortiumChaincodes|系统规定参数。取值：**DescribeFabricConsortiumChaincodes**。

 |
|ConsortiumId|String|是|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

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
|Result| | |联盟的链码列表

 |
|ChaincodeId|String|code-sacc-1pr09q7jmo0np|链码ID

 |
|ChaincodeName|String|sacc|链码名称

 |
|ChaincodeVersion|String|1.0|链码版本

 |
|ChannelId|String|chan-channelx-1l1hmckuuisxo|通道ID

 |
|ChannelName|String|cname|通道名

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

 |
|CreateTime|String|1544411108000|创建时间

 |
|DeployTime|String|1544411108000|部署时间

 |
|EndorsePolicy|String|OR \('aaaaaa1MSP.peer'\)|背书策略

 |
|Input|String|input|链码输入

 |
|Install|Boolean|true|是否安装

 |
|Message|String|ok|消息

 |
|Path|String|go-sdk-demo/chaincode/src|链码路径

 |
|ProviderId|String|peers-aaaaaa2-1eqnj5o5w9dt3|链码上传者ID

 |
|ProviderName|String|name|链码上传者名称

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

http(s)://[Endpoint]/?Action=DescribeFabricConsortiumChaincodes
&ConsortiumId=consortium-lianmenyumingyi-hc5d1bwlulg7
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricConsortiumChaincodesResponse>
  <Result>
		    <ChaincodeName>asset_mgmtv1.0.out</ChaincodeName>
		    <ChannelId>chan-channel1-1180moa11f7g5a</ChannelId>
		    <Install>false</Install>
		    <State>Checking</State>
		    <ConsortiumId>consortium-testthree-3i6j6d8ian5668</ConsortiumId>
		    <Type>0</Type>
		    <CreateTime>2018-07-31T08:13:27.000+0000</CreateTime>
		    <ProviderId>peers-test3-25c96n9n6jh3dc</ProviderId>
		    <ChannelName>channel1</ChannelName>
		    <ChaincodeVersion>unknown</ChaincodeVersion>
		    <EndorsePolicy>OR (&amp;#test3MSP.member&amp;#39;)</EndorsePolicy>
		    <ChaincodeId>code-asset_mgmtv1.0.out-1gab808kn8bfgl</ChaincodeId>
	  </Result>
	  <RequestId>66495305-6EE5-4023-96F2-93B47B79E076</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricConsortiumChaincodesResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"ChannelId":"chan-channel1-1180moa11f7g5a",
			"ChaincodeVersion":"unknown",
			"ConsortiumId":"consortium-testthree-3i6j6d8ian5668",
			"State":"Checking",
			"Install":false,
			"ChaincodeName":"asset_mgmtv1.0.out",
			"Type":0,
			"ProviderId":"peers-test3-25c96n9n6jh3dc",
			"CreateTime":"2018-07-31T08:13:27.000+0000",
			"ChannelName":"channel1",
			"EndorsePolicy":"OR (&#test3MSP.member&#39;)",
			"ChaincodeId":"code-asset_mgmtv1.0.out-1gab808kn8bfgl"
		}
	],
	"RequestId":"66495305-6EE5-4023-96F2-93B47B79E076",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

