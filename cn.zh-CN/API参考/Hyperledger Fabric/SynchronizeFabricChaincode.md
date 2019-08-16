# SynchronizeFabricChaincode {#doc_api_Baas_SynchronizeFabricChaincode .reference}

调用SynchronizeFabricChaincode同步链码的升级和实例化的状态。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=SynchronizeFabricChaincode&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|SynchronizeFabricChaincode|系统规定参数。取值：**SynchronizeFabricChaincode**。

 |
|ChaincodeId|String|是|code-sacc-1pr09q7jm\*\*\*\*|链码ID

 |
|OrganizationId|String|是|peers-aaaaaa2-1eqnj5o5w\*\*\*\*|组织ID

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
|ChaincodeId|String|code-sacc-1pr09q7jm\*\*\*\*|链码ID

 |
|ChaincodeName|String|mychaincode|链码名

 |
|ChaincodeVersion|String|1.0|链码版本

 |
|ChannelName|String|chan-channelx-1l1hmckuuisxo|通道名

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwl\*\*\*\*|联盟ID

 |
|CreateTime|String|1533025590|创建时间

 |
|DeployTime|String|1533025590|部署时间

 |
|EndorsePolicy|String|OR \('aaaaaa1MSP.peer'\)|背书策略

 |
|Input|String|input|输入

 |
|Install|Boolean|false|是否安装

 |
|Message|String|ok|信息

 |
|Path|String|go-sdk-demo/chaincode/src|路径

 |
|ProviderId|String|provider|上传者ID

 |
|ProviderName|String|name|上传者

 |
|State|String|Running|状态

 |
|Type|Integer|1|类型

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=SynchronizeFabricChaincode
&ChaincodeId=code-sacc-1pr09q7jm****
&OrganizationId=peers-aaaaaa2-1eqnj5o5w****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<SynchronizeFabricChaincodeResponse>
  <Result>
		    <ProviderId>provider</ProviderId>
		    <ProviderName>name</ProviderName>
		    <ChaincodeName>mycc3</ChaincodeName>
		    <Input>args:&amp;quot;john&amp;quot; args:&amp;quot;10&amp;quot; </Input>
		    <Install>false</Install>
		    <State>Running</State>
		    <Type>1</Type>
		    <ChannelName>mychannel</ChannelName>
		    <ConsortiumId>consortium-lianmenyumingyi-hc5d1bwl****</ConsortiumId>
		    <ChaincodeVersion>0.1</ChaincodeVersion>
		    <ChaincodeId>cc-null-c856k9i1m****</ChaincodeId>
		    <Path>github.com/hyperledger/fabric-samples/chaincode/sacc</Path>
	  </Result>
	  <RequestId>2A3ABD81-95F5-4931-ACB3-31BDAE561FC7</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</SynchronizeFabricChaincodeResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":{
		"ChaincodeVersion":"0.1",
		"Input":"args:&quot;john&quot; args:&quot;10&quot; ",
		"ConsortiumId":"consortium-lianmenyumingyi-hc5d1bwl****",
		"State":"Running",
		"Install":false,
		"ChaincodeName":"mycc3",
		"Type":1,
		"ProviderName":"name",
		"ProviderId":"provider",
		"ChannelName":"mychannel",
		"Path":"github.com/hyperledger/fabric-samples/chaincode/sacc",
		"ChaincodeId":"cc-null-c856k9i1m****"
	},
	"RequestId":"2A3ABD81-95F5-4931-ACB3-31BDAE561FC7",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

