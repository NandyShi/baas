# InstallFabricChaincode {#doc_api_Baas_InstallFabricChaincode .reference}

调用InstallFabricChaincode安装链码。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=InstallFabricChaincode&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|InstallFabricChaincode|系统规定参数。取值：**InstallFabricChaincode**。

 |
|ChaincodeId|String|是|chan-channelx-1l1hmckuuisxo|链码ID

 |
|OrganizationId|String|是|peers-aaaaaa2-1eqnj5o5w9dt3|组织ID

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
|ChaincodeId|String|cc-198jejf8f8chi8|链码ID

 |
|ChaincodeName|String|mychannel|链码名称

 |
|ChaincodeVersion|String|1.0|链码版本

 |
|ChannelName|String|mychannel|通道名

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

 |
|CreateTime|String|1533025590|创建时间

 |
|DeployTime|String|1533025590|部署时间

 |
|EndorsePolicy|String|OR \("perf9141MSP.member"\)|背书策略

 |
|Input|String|input|输入

 |
|Install|Boolean|false|是否安装

 |
|Message|String|ok|信息

 |
|Path|String|github.com/hyperledger/fabric-samples/chaincode/sacc|路径

 |
|ProviderId|String|providerid|上传者ID

 |
|ProviderName|String|prividername|上传者

 |
|State|String|Pending|状态

 |
|Type|Integer|1|类型

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=InstallFabricChaincode
&ChaincodeId=chan-channelx-1l1hmckuuisxo
&OrganizationId=peers-aaaaaa2-1eqnj5o5w9dt3
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<InstallFabricChaincodeResponse>
  <Result>
		    <install>false</install>
		    <channelName>mychannel</channelName>
		    <input>args:&amp;quot;john&amp;quot; args:&amp;quot;10&amp;quot; </input>
		    <ChaincodeName>mycc3</ChaincodeName>
		    <Path>github.com/hyperledger/fabric-samples/chaincode/sacc</Path>
		    <state>Running</state>
		    <chaincodeId>cc-198jejf8f8chi8</chaincodeId>
		    <type>1</type>
		    <ChaincodeVersion>0.1</ChaincodeVersion>
		    <ConsortiumId>consortium-lianmenyumingyi-hc5d1bwlulg7</ConsortiumId>
		    <CreateTime>1533025590</CreateTime>
		    <EndorsePolicy>OR (perf9141MSP.member)</EndorsePolicy>
		    <Message>OK</Message>
	  </Result>
	  <RequestId>7D27692E-C501-4B1D-878C-0B869DD3D9E6</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</InstallFabricChaincodeResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"install":false,
		"channelName":"mychannel",
		"ConsortiumId":"consortium-lianmenyumingyi-hc5d1bwlulg7",
		"Message":"OK",
		"state":"Running",
		"chaincodeId":"cc-198jejf8f8chi8",
		"type":1,
		"EndorsePolicy":"OR (perf9141MSP.member)",
		"Path":"github.com/hyperledger/fabric-samples/chaincode/sacc",
		"ChaincodeVersion":"0.1",
		"input":"args:&quot;john&quot; args:&quot;10&quot; ",
		"ChaincodeName":"mycc3",
		"CreateTime":"1533025590"
	},
	"RequestId":"7D27692E-C501-4B1D-878C-0B869DD3D9E6",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

