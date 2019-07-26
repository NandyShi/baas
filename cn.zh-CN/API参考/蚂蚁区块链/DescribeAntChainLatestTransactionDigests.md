# DescribeAntChainLatestTransactionDigests {#doc_api_Baas_DescribeAntChainLatestTransactionDigests .reference}

查询一条蚂蚁区块链最新的交易摘要列表

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainLatestTransactionDigests&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|AntChainId|String|是|pYogqb9v|区块链ID

 |
|Action|String|否|DescribeAntChainLatestTransactionDigests|系统规定参数。取值：DescribeAntChainLatestTransactionDigests。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainLatestTransactionDigests
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"3348160E-187B-47BD-B1B9-76AD4AFA4558",
	"data":{
		"Result":[
			{
				"to":"0f7256e0886e2095f328a244cf44823f95a82dedb3e51a1f46f8c272cf1c6030",
				"createTime":1563861357920,
				"hash":"945ffb5e2a8aaf41eed862f7c1565603683b7a640b7b78a168396897979335a9",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"FREEZE_ACCOUNT_CONTRACT"
			},
			{
				"to":"0f7256e0886e2095f328a244cf44823f95a82dedb3e51a1f46f8c272cf1c6030",
				"createTime":1563861353157,
				"hash":"5d379f516bf8f96991ee80d91504cfbf94f0b2feb87b375d07d04b019fd7bb3f",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"UNFREEZE_ACCOUNT_CONTRACT"
			},
			{
				"to":"8e35c2cd3bf6641bdb0e2050b76932cbb2e6034a0ddacc1d9bea82a6ba57f7cf",
				"createTime":1563861343692,
				"hash":"50df783d3e0038ee2ebf62c2295e19da9f95fc99dca6d9de4c0bf8f109c2a2f1",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"FREEZE_ACCOUNT_CONTRACT"
			},
			{
				"to":"4db58ada9221304b161ab0aa11b032a62d60d9ab29e41c6d238f4401c81c8189",
				"createTime":1563861340667,
				"hash":"7f299376af6e44825b55dca4c840d7f7bdc124984adfa2501b3ba5d7f3afb61b",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"UNFREEZE_ACCOUNT_CONTRACT"
			},
			{
				"to":"8e35c2cd3bf6641bdb0e2050b76932cbb2e6034a0ddacc1d9bea82a6ba57f7cf",
				"createTime":1563861331665,
				"hash":"2a185f80ea614459f7d2125e0ff43c68f96bfc4266b737646ef8250562b71aca",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"UNFREEZE_ACCOUNT_CONTRACT"
			},
			{
				"to":"49f3bd00a75b5b7519965014a37f14362cc88e303ed9615a49bc888e841184ed",
				"createTime":1563861325469,
				"hash":"944831a05c11be9290ffbe2b29734234462da0fed0192b661c42846d18bdb9f7",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"UNFREEZE_ACCOUNT_CONTRACT"
			},
			{
				"to":"0f7256e0886e2095f328a244cf44823f95a82dedb3e51a1f46f8c272cf1c6030",
				"createTime":1563861322053,
				"hash":"5d7da0043114b58488e0867c8dddb8b35812ce6e198235ef70d58d06d843024f",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"FREEZE_ACCOUNT_CONTRACT"
			},
			{
				"to":"8e35c2cd3bf6641bdb0e2050b76932cbb2e6034a0ddacc1d9bea82a6ba57f7cf",
				"createTime":1563861318974,
				"hash":"0c94292b144c69cbdc01389938f660a430dda1a50369de3a2c92b08d7e61f145",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"FREEZE_ACCOUNT_CONTRACT"
			},
			{
				"to":"4db58ada9221304b161ab0aa11b032a62d60d9ab29e41c6d238f4401c81c8189",
				"createTime":1563861316016,
				"hash":"293a7412174f7827135ae0610f85f4bc2d7eca21aca017935c3cd048a30dc2b4",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"FREEZE_ACCOUNT_CONTRACT"
			},
			{
				"to":"4db58ada9221304b161ab0aa11b032a62d60d9ab29e41c6d238f4401c81c8189",
				"createTime":1563861312633,
				"hash":"21f5977f5f9103c251968e4f84c0e1d3c68549a25b185e21791cb5ad5a4839f6",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"UNFREEZE_ACCOUNT_CONTRACT"
			},
			{
				"to":"8e35c2cd3bf6641bdb0e2050b76932cbb2e6034a0ddacc1d9bea82a6ba57f7cf",
				"createTime":1563861307139,
				"hash":"78329f5dd5af3ab2de339980fef05a0aa1d50ad1ddbce247d4d1e8e85cc5222f",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"UNFREEZE_ACCOUNT_CONTRACT"
			},
			{
				"to":"49f3bd00a75b5b7519965014a37f14362cc88e303ed9615a49bc888e841184ed",
				"createTime":1563861302697,
				"hash":"e089544b7a9e5354ea4ac57769d854acc0c79acee54420c9232924d978601969",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"FREEZE_ACCOUNT_CONTRACT"
			},
			{
				"to":"e93372533f323b2f12783aa3a586135cf421486439c2cdcde47411b78f9839ec",
				"createTime":1563765546000,
				"hash":"e0a27e8b0bd0d3053b29c133f257f636c37cb1ba8524684e3bfc6f7a48191494",
				"from":"e7d3e769f3f593dadcb8634cc5b09fc90dd3a61c4a06a79cb0923662fe6fae6b",
				"transactionV10Type":"CALL_CONTRACT"
			}
		],
		"RequestId":"3348160E-187B-47BD-B1B9-76AD4AFA4558"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

