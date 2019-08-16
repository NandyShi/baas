# DescribeFabricConsortiumOrderers {#doc_api_Baas_DescribeFabricConsortiumOrderers .reference}

调用DescribeFabricConsortiumOrderers获取联盟的Orderer列表。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeFabricConsortiumOrderers&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DescribeFabricConsortiumOrderers|系统规定参数。取值：**DescribeFabricConsortiumOrderers**。

 |
|ConsortiumId|String|是|consortium-aaaaaa-akpcsjjac2jd|联盟ID

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
|Result| | |联盟的Orderer列表

 |
|CreateTime|String|1544411108000|创建时间

 |
|Domain|String|domain|域名

 |
|InstanceType|String|ecs.n1.small|实例类型

 |
|OrdererName|String|order1|Orderer名称

 |
|Port|Integer|7050|端口

 |
|UpdateTime|String|1544411108000|更新时间

 |
|Success|Boolean|true|是否成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeFabricConsortiumOrderers
&ConsortiumId=consortium-aaaaaa-akpcsjjac2jd	
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DescribeFabricConsortiumOrderersResponse>
  <Result>
		    <OrdererName>order1</OrdererName>
		    <Port>7050</Port>
		    <Domain>ordasdaerer1.orzxczcZXXweqwxsczxzXcxzxXzg1.alumunum.com</Domain>
		    <CreateTime>2018-07-01 09:00:00</CreateTime>
		    <UpdateTime>2018-07-02 09:00:00</UpdateTime>
		    <InstanceType>ecs.n1.small</InstanceType>
	  </Result>
	  <Result>
		    <OrdererName>order2</OrdererName>
		    <Port>7050</Port>
		    <Domain>orderer2.org1.alumunum.com</Domain>
		    <CreateTime>2018-07-01 09:00:00</CreateTime>
		    <UpdateTime>2018-07-02 09:00:00</UpdateTime>
		    <InstanceType>ecs.n1.small</InstanceType>
	  </Result>
	  <RequestId>98B37CF5-AB0C-423E-8335-81A54899577E</RequestId>
	  <Success>true</Success>
	  <ErrorCode>200</ErrorCode>
</DescribeFabricConsortiumOrderersResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"Result":[
		{
			"Port":7050,
			"Domain":"ordasdaerer1.orzxczcZXXweqwxsczxzXcxzxXzg1.alumunum.com",
			"CreateTime":"2018-07-01 09:00:00",
			"UpdateTime":"2018-07-02 09:00:00",
			"OrdererName":"order1",
			"InstanceType":"ecs.n1.small"
		},
		{
			"Port":7050,
			"Domain":"orderer2.org1.alumunum.com",
			"CreateTime":"2018-07-01 09:00:00",
			"UpdateTime":"2018-07-02 09:00:00",
			"OrdererName":"order2",
			"InstanceType":"ecs.n1.small"
		}
	],
	"RequestId":"98B37CF5-AB0C-423E-8335-81A54899577E",
	"ErrorCode":200,
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

