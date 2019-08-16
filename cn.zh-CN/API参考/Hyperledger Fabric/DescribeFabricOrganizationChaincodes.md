# DescribeFabricOrganizationChaincodes {#doc_api_Baas_DescribeFabricOrganizationChaincodes .reference}

调用DescribeFabricOrganizationChaincodes获取组织的链码列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricOrganizationChaincodes&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricOrganizationChaincodes|系统规定参数。取值：**DescribeFabricOrganizationChaincodes**。

 |
|OrganizationId|String|是|peers-aaaaaa2-1eqnj5o5w\*\*\*\*|组织ID

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
|RequestId|String|1890FA4F-067A-4CE9-AC9B-2BD2E58FB5D3|请求ID

 |
|Result| | |组织的链码列表

 |
|ChaincodeId|String|code-sacc-1pr09q7jmo0np|链码ID

 |
|ChaincodeName|String|mycc|链码名

 |
|ChaincodeVersion|String|0.3|链码版本

 |
|ChannelId|String|chan-first-channel-31hlgpen5k5lig|通道ID

 |
|ChannelName|String|first-channel|通道名

 |
|ConsortiumId|String|consortium-lianmenyumingyi-hc5d1bwlulg7|联盟ID

 |
|CreateTime|String|1533025590|创建时间

 |
|Creator|String|uid-23425|创建者

 |
|DeployTime|String|1533025590|部署时间

 |
|EndorsePolicy|String|OR \(&\#39;perf9141MSP.member&\#39;\)|背书策略

 |
|Installed|String|Installed|是否安装

 |
|Message|String|OK|消息

 |
|State|String|Running|状态。取值：

 -   **CHECKING**
-   **ERROR**
-   **INSTALLABLE**
-   **INSTALLED**
-   **RUNNING**
-   **UPGRADABLE**

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricOrganizationChaincodes
&OrganizationId=peers-aaaaaa2-1eqnj5o5w****
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricOrganizationChaincodesResponse>
  <Result>
			    <ChaincodeName>sacc</ChaincodeName>
			    <ChannelId>chan-first-channel-31hlgpen5k5lig</ChannelId>
			    <State>Instantiatable</State>
			    <ConsortiumId>10000</ConsortiumId>
			    <Creator>perf9141</Creator>
			    <CreateTime>2018-08-19T02:00:21.000+0000</CreateTime>
			    <Installed>Installed</Installed>
			    <DeployTime>2018-08-19T08:24:32.000+0000</DeployTime>
			    <ChannelName>first-channel</ChannelName>
			    <ChaincodeVersion>1.0.6</ChaincodeVersion>
			    <EndorsePolicy>OR (&amp;#39;perf914MSP.member&amp;#39;)</EndorsePolicy>
			    <ChaincodeId>code-sacc-1ai2bl61ggb6bf</ChaincodeId>
		        <Message>OK</Message>
          </Result>
		  <Result>
			    <ChaincodeName>sacc</ChaincodeName>
			    <ChannelId>chan-first-channel-31hlgpen5k5lig</ChannelId>
			    <State>Upgradable</State>
			    <ConsortiumId>10000</ConsortiumId>
			    <Creator>perf9143</Creator>
			    <CreateTime>2018-08-19T02:15:54.000+0000</CreateTime>
			    <Installed>Installed</Installed>
			    <ChannelName>first-channel</ChannelName>
			    <ChaincodeVersion>1.0.7</ChaincodeVersion>
			    <EndorsePolicy>OR (&amp;#39;perf9143MSP.member&amp;#39;)</EndorsePolicy>
			    <ChaincodeId>code-sacc-a236mc8gmk9m9</ChaincodeId>
		        <Message>OK</Message>
          </Result>
		  <RequestId>C741EF76-4F31-40BF-B286-E87C9D3E7232</RequestId>
		  <Success>true</Success>
		  <ErrorCode>200</ErrorCode>
</DescribeFabricOrganizationChaincodesResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"ConsortiumId":"10000",
			"Message":"OK",
			"Creator":"perf9143",
			"DeployTime":"2018-08-19T08:43:26.000+0000",
			"ChannelName":"first-channel",
			"EndorsePolicy":"OR (&#39;perf9143MSP.member&#39;)",
			"ChannelId":"chan-first-channel-31hlgpen5k5lig",
			"ChaincodeVersion":"1.0.10",
			"ChaincodeName":"sacc",
			"State":"Upgradable",
			"CreateTime":"2018-08-19T08:37:33.000+0000",
			"Installed":"Installed",
			"ChaincodeId":"code-sacc-nbk70pidp2jm7"
		},
		{
			"ConsortiumId":"10000",
			"Message":"OK",
			"Creator":"perf9141",
			"DeployTime":"2018-08-19T08:46:02.000+0000",
			"ChannelName":"first-channel",
			"EndorsePolicy":"OR (&#39;perf9141MSP.member&#39;)",
			"ChannelId":"chan-first-channel-31hlgpen5k5lig",
			"ChaincodeVersion":"1.0.11",
			"ChaincodeName":"sacc",
			"State":"Upgradable",
			"CreateTime":"2018-08-19T08:38:18.000+0000",
			"Installed":"Installed",
			"ChaincodeId":"code-sacc-2bpegdo9mfchod"
		}
	],
	"RequestId":"C741EF76-4F31-40BF-B286-E87C9D3E7232",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

