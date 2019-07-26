# DescribeAntChainContractProjectContentTree {#doc_api_Baas_DescribeAntChainContractProjectContentTree .reference}

获取一个合约工程的内容树

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Baas&api=DescribeAntChainContractProjectContentTree&type=RPC&version=2018-12-21)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|ProjectId|String|是|2L9VK68g|项目ID

 |
|Action|String|否|DescribeAntChainContractProjectContentTree|系统规定参数。取值：DescribeAntChainContractProjectContentTree。

 |
|RegionId|String|否|cn-hangzhou|地域ID

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|A0DF307A-A44A-476F-99D8-BA4F205350BD|请求ID

 |
|Result| | |请求结果

 |
|Children| |\[\]|子文件

 |
|ProjectDescription|String|description|工程描述

 |
|ProjectId|String|2L9VK68g|工程ID

 |
|ProjectName|String|projectname|工程名称

 |
|ProjectVersion|String|5|工程版本

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DescribeAntChainContractProjectContentTree
&<公共请求参数>

```

正常返回示例

`JSON` 格式

``` {#json_return_success_demo}
{
	"successResponse":true,
	"requestId":"A0DF307A-A44A-476F-99D8-BA4F205350BD",
	"data":{
		"Result":{
			"ProjectDescription":"",
			"ProjectName":"projectname",
			"ProjectVersion":"5",
			"Children":[
				{
					"id":"bz9kr4X2",
					"gmtModified":1563937111000,
					"gmtCreate":1563937111000,
					"directory":true,
					"name":"wenjianjia",
					"children":[
						{
							"content":"",
							"id":"5m91BL8Y",
							"gmtModified":1563954481000,
							"parentId":"bz9kr4X2",
							"gmtCreate":1563954481000,
							"directory":false,
							"name":"ads",
							"children":[],
							"projectId":"2L9VK68g"
						}
					],
					"projectId":"2L9VK68g"
				},
				{
					"content":"",
					"id":"broOrJ8k",
					"gmtModified":1563937114000,
					"gmtCreate":1563869464000,
					"directory":false,
					"name":"123",
					"children":[],
					"projectId":"2L9VK68g"
				},
				{
					"content":"pragma solidity ^0.4.23;\n// We have to specify which version of compiler this code will compile with, \n// version should be lower than (or equals to) the supported version showing on this tool.\ncontract Voting {\n    /* Solidity doesn't let you pass in an array of strings in the constructor (yet).\n    We will use an array of bytes32 instead to store the list of candidates with string type.\n    */\n    bytes32[] public candidateList;\n\n    FDGGFDGFDGFDGFDGFDGFDGFDGFDGFD\n    mapping (bytes32 => uint8) public votesReceived;\n\n    /* Counting for candidate counts and total votes for all candidates\n    */\n    uint256 public candidateCount;\n    uint256 public totalVotes;\n\n\n    /* Events which will help for logging and debugging\n    'identity' is like 'address' in original Solidity, length of 'identity' is 256 (bits).\n    */\n    event VOTE(bytes32 candidate, identity voterId);\n    event VALID(bool valid);\n\n\n    /* This is the constructor which will be called once when you\n    deploy the contract to the blockchain. When we deploy the contract,\n    we will pass an array of candidates who will be contesting in the election.\n    You can input a candidate name like: Mike , it will be converted to bytes32.\n    */\n    constructor(bytes32[] candidateNames) public {\n        candidateList = candidateNames;\n        candidateCount = candidateList.length;\n    }\n\n    // This function returns the total votes a candidate has received so far.\n    function totalVotesFor(bytes32 candidate) view public returns (uint8) {\n        require(validCandidate(candidate));\n        return votesReceived[candidate];\n    }\n\n    // This function increments the vote count for the specified candidate. \n    // This is equivalent to casting a vote.\n    function voteForCandidate(bytes32 candidate) public {\n        require(validCandidate(candidate));\n        votesReceived[candidate] += 1;\n        totalVotes += 1;\n    \n        emit VOTE(candidate, msg.sender);\n    }\n\n    // This function will help to check whether target candidate is in the candidateList.\n    function validCandidate(bytes32 candidate) view public returns (bool) {\n        for (uint i = 0; i < candidateList.length; i++) {\n            if (candidateList[i] == candidate) {\n            emit VALID(true);\n            return true;\n            }\n        }\n        emit VALID(false);\n        return false;\n    }\n}",
					"id":"1q8Bv68p",
					"gmtModified":1563860292000,
					"gmtCreate":1562847564000,
					"directory":false,
					"name":"demo.sol",
					"children":[],
					"projectId":"2L9VK68g"
				},
				{
					"content":"",
					"id":"GKX7KZX0",
					"gmtModified":1563954499000,
					"gmtCreate":1563954499000,
					"directory":false,
					"name":"test",
					"children":[],
					"projectId":"2L9VK68g"
				}
			],
			"ProjectId":"2L9VK68g"
		},
		"RequestId":"A0DF307A-A44A-476F-99D8-BA4F205350BD"
	},
	"code":"200"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/Baas)查看更多错误码。

