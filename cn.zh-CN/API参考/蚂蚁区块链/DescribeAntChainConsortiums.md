# DescribeAntChainConsortiums {#doc_api_Baas_DescribeAntChainConsortiums .reference}

获取联盟列表

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainConsortiums&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|PageNumber|Integer|是|1|页面编号

 |
|PageSize|Integer|是|10|每页显示条例数

 |
|Action|String|否|DescribeAntChainConsortiums|系统规定参数。取值：DescribeAntChainConsortiums。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|D68D66B6-1964-4073-8714-B49F5EF1AEFC|请求ID

 |
|Result| | |请求结果

 |
|AntConsortiums| | |蚂蚁区块链联盟

 |
|ChainNum|Long|1|联盟内区块链梳理

 |
|ConsortiumDescription|String|测试联盟|联盟描述

 |
|ConsortiumId|String|DV80nJXq|联盟ID

 |
|ConsortiumName|String|第一个联盟|联盟名称

 |
|CreateTime|Long|1562845453000|联盟创建时戳

 |
|MemberNum|Long|2|联盟成员数量

 |
|Role|String|SuperAdmin|账户身份角色

 |
|Status|String|Active|联盟状态

 |
|Pagination| | |分页情况

 |
|PageNumber|Integer|1|页码

 |
|PageSize|Integer|10|每页展示条例数

 |
|TotalCount|Integer|1|联盟个数

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainConsortiums
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<xml version="1.0" encoding="UTF-8">
	  <code>200</code>
	  <data>
		    <RequestId>D68D66B6-1964-4073-8714-B49F5EF1AEFC</RequestId>
		    <Result>
			      <Pagination>
				        <TotalCount>3</TotalCount>
				        <PageSize>10</PageSize>
				        <PageNumber>1</PageNumber>
			      </Pagination>
			      <AntConsortiums>
				        <Status>Active</Status>
				        <Role>SuperAdmin</Role>
				        <ConsortiumId>DV80nJXq</ConsortiumId>
				        <ChainNum>1</ChainNum>
				        <CreateTime>1562845453000</CreateTime>
				        <ConsortiumDescription>测试联盟</ConsortiumDescription>
				        <ConsortiumName>第一个联盟</ConsortiumName>
				        <MemberNum>2</MemberNum>
			      </AntConsortiums>
		    </Result>
	  </data>
	  <requestId>D68D66B6-1964-4073-8714-B49F5EF1AEFC</requestId>
	  <successResponse>true</successResponse>
</xml>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"D68D66B6-1964-4073-8714-B49F5EF1AEFC",
	"data":{
		"Result":{
			"Pagination":{
				"PageNumber":1,
				"TotalCount":1,
				"PageSize":10
			},
			"AntConsortiums":[
				{
					"ConsortiumName":"第一个联盟",
					"Status":"Active",
					"MemberNum":2,
					"ChainNum":1,
					"ConsortiumId":"DV80nJXq",
					"CreateTime":1562845453000,
					"Role":"SuperAdmin",
					"ConsortiumDescription":"测试联盟"
				}
			]
		},
		"RequestId":"D68D66B6-1964-4073-8714-B49F5EF1AEFC"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

