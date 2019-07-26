# DescribeAntChainMembers {#doc_api_Baas_DescribeAntChainMembers .reference}

获取联盟成员列表

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainMembers&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ConsortiumId|String|是|q0oWq92P|联盟ID

 |
|PageNumber|Integer|是|1|页面编号

 |
|PageSize|Integer|是|10|页面包含条例数

 |
|Action|String|否|DescribeAntChainMembers|系统规定参数。取值：DescribeAntChainMembers。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|E0DB75A2-28C8-4295-8851-A157FFB3DFED|请求ID

 |
|Result| | |请求结果

 |
|Members| | |联盟成员

 |
|JoinTime|Long|1557477823000|成员加入联盟时戳

 |
|MemberId|String|uid-1388601577407805|成员ID

 |
|MemberName|String|uid-1562589998337656|成员名称

 |
|Role|String|Member|成员身份

 |
|Status|String|AllianceNotJoined|加入联盟状态

 |
|Pagination| | |分页信息

 |
|PageNumber|Integer|1|页面编号

 |
|PageSize|Integer|10|每页数量

 |
|TotalCount|Integer|6|总数

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainMembers
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<xml version="1.0" encoding="UTF-8">
	  <code>200</code>
	  <data>
		    <RequestId>E0DB75A2-28C8-4295-8851-A157FFB3DFED</RequestId>
		    <Result>
			      <Pagination>
				        <PageSize>10</PageSize>
				        <Total>2</Total>
				        <Current>1</Current>
			      </Pagination>
			      <Members>
				        <Status>AllianceJoined</Status>
				        <Role>SuperAdmin</Role>
				        <MemberId>uid-1388601577407805</MemberId>
				        <UserId>OYXLOokN</UserId>
				        <JoinTime>1557477823000</JoinTime>
				        <MemberName>uid-1388601577407805sss</MemberName>
			      </Members>
			      <Members>
				        <Status>AllianceNotJoined</Status>
				        <Role>Member</Role>
				        <MemberId>uid-1562589998337656</MemberId>
				        <UserId>broOV8kD</UserId>
				        <JoinTime>1560147228000</JoinTime>
				        <MemberName>uid-1562589998337656</MemberName>
			      </Members>
		    </Result>
	  </data>
	  <requestId>E0DB75A2-28C8-4295-8851-A157FFB3DFED</requestId>
	  <successResponse>true</successResponse>
</xml>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"15EFC35E-3DAD-4E97-A97D-9F81660C9DE9",
	"data":{
		"Result":{
			"Pagination":{
				"PageNumber":1,
				"TotalCount":6,
				"PageSize":10
			},
			"Members":[
				{
					"Status":"AllianceJoined",
					"JoinTime":1562845453000,
					"Role":"SuperAdmin",
					"MemberName":"uid-1287126353308684",
					"MemberId":"1287126353308684"
				},
				{
					"Status":"AllianceNotJoined",
					"JoinTime":1562847689000,
					"Role":"Member",
					"MemberName":"uid-1897759808932113",
					"MemberId":"1897759808932113"
				},
				{
					"Status":"AllianceNotJoined",
					"JoinTime":1562847826000,
					"Role":"Member",
					"MemberName":"uid-1244631294173906",
					"MemberId":"1244631294173906"
				},
				{
					"Status":"AllianceJoined",
					"JoinTime":1562848743000,
					"Role":"Member",
					"MemberName":"uid-1298430932251201",
					"MemberId":"1298430932251201"
				},
				{
					"Status":"AllianceNotJoined",
					"JoinTime":1562848777000,
					"Role":"Member",
					"MemberName":"uid-1908162809538613",
					"MemberId":"1908162809538613"
				},
				{
					"Status":"AllianceNotJoined",
					"JoinTime":1562850385000,
					"Role":"Member",
					"MemberName":"uid-100",
					"MemberId":"100"
				}
			]
		},
		"RequestId":"15EFC35E-3DAD-4E97-A97D-9F81660C9DE9"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

