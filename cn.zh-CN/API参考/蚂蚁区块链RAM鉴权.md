# 蚂蚁区块链RAM鉴权 {#concept_2151252 .concept}

在使用RAM账号调用蚂蚁区块链服务API前，需要主账号通过创建授权策略对RAM账号进行授权。在授权策略中，使用资源描述符（Alibaba Cloud Resource Name，ARN）指定授权资源。

本文提供了在蚂蚁区块链服务中通过访问控制实现团队或者部门成员鉴权、跨账号资源授权以及跨云服务授权的RAM鉴权规则。在了解如何使用访问控制RAM授权和访问区块链服务之前，确保您已阅读了[RAM产品文档](https://help.aliyun.com/document_detail/28627.html#concept-oyr-zzv-tdb)和[RAM API文档](https://help.aliyun.com/document_detail/62184.html#concept-vdd-rmk-xdb)。

## 可授权的蚂蚁区块链资源类型 {#section_kdd_ukz_u3w .section}

在进行RAM子账号授权时，蚂蚁区块链资源的描述方式如下：

|资源类型|授权策略中的资源描述方法|
|----|------------|
|联盟|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId|
|区块链|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|合约工程|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/contractProject/$projectId|

其中，`$consortiumId`为联盟Id，`$blockchainId`为区块链Id，`$projectId`为联盟内的合约工程Id。

## 可授权的蚂蚁区块链接口 {#section_6pz_q07_990 .section}

下表列举了蚂蚁区块链中可授权的API及其描述方式：

|API|资源描述|
|---|----|
|CreateAntChainConsortium|acs:baas:\*:$accountId:antChainConsortium/\*|
|DescribeAntChainConsortiums|acs:baas:\*:$accountId:antChainConsortium/\*|
|UpdateAntChainConsortium|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId|
|DeleteAntChainConsortium|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId|
|InviteAntChainMember|acs:baas:\*:$accountId:\*|
|AgreeAntChainInvitation|acs:baas:\*:$accountId:\*|
|DescribeAntChainMembers|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId|
|UpdateAntChainMember|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId|
|DescribeAntChains|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/\*|
|CreateAntChain|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/\*|
|UpdateAntChain|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|ApplyAntChainCertificate|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|ApplyAntChainCertificateWithKeyAutoCreation|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|DescribeAntChainDownloadPaths|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|ResetAntChainCertificate|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|DescribeAntChainLatestBlocks|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|DescribeAntChainLatestTransactionDigests|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|DescribeAntChainInformation|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|DescribeAntChainTransactionStatistics|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|DescribeAntChainBlock|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|DescribeAntChainTransaction|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|DescribeAntChainTransactionReceipt|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|ResetAntChainUserCertificate|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|DescribeAntChainAccounts|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|DescribeAntChainNodes|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|CreateAntChainAccount|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|CreateAntChainAccountWithKeyPairAutoCreation|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|FreezeAntChainAccount|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|UnfreezeAntChainAccount|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|DescribeAntChainCertificateApplications|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/blockchain/$blockchainId|
|CreateAntChainContractProject|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/contractProject/\*|
|CopyAntChainContractProject|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/contractProject/\*|
|DeleteAntChainContractProject|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/contractProject/$projectId|
|UpdateAntChainContractProject|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/contractProject/$projectId|
|DescribeAntChainContractProjects|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/contractProject/\*|
|DescribeAntChainContractProjectContentTree|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/contractProject/$projectId|
|CreateAntChainContractContent|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/contractProject/$projectId|
|DeleteAntChainContractContent|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/contractProject/$projectId|
|UpdateAntChainContractContent|acs:baas:\*:$consortiumOwnerUid:antChainConsortium/$consortiumId/contractProject/$projectId|
|DescribeCloudIDEEnvConfigs|acs:baas:\*:$accountId:\*|
|ProcessCloudIDEContractTransaction|acs:baas:\*:$accountId:\*|
|概览页面体验链相关接口|符合不鉴权条件，不进行RAM鉴权。|
|DescribeAntChainRegions|该接口不进行RAM鉴权。|

## 蚂蚁区块链RAM规则示例 {#section_419_qww_zo4 .section}

例1 ：授权BaaS服务只读类操作。这种类型的权限能够允许用户通过控制台或API查看区块链状态，下载SDK。

``` {#codeblock_hb7_qyx_73n}
{

   "Statement": [{

       "Action": ["baas:DescribeAntChain*"],

        "Effect": "Allow",

        "Resource": "acs:baas:*:*:*"

   }],

   "Version": "1"

}
```

例2：授权联盟管理类操作（查询，创建、更新、删除）。这种类型的权限允许用户通过控制台或API管理联盟。

``` {#codeblock_v0v_9de_eb0}
{

  "Statement": [{

     "Action": "baas:*AntChainConsortium*",

     "Effect": "Allow",
     "Resource": ["acs:baas:*:*:antChainConsortium/*"]

  }],

  "Version": "1"

}
```

例3：更精细化的链码开发者授权。该权限通常需要全部的读类型操作，以及特定联盟的资源管理类操作。按照最小权限原则，以合约管理功能为例，需要限制该用户仅能对用于指定联盟的指定合约工程进行操作。将下面的`antChainConsortium/$consortiumId/contractProject/$projectId`替换为具体资源在区块链服务中的资源Id。

``` {#codeblock_xm2_h67_ng0}
{

 "Statement": [{

   "Action": ["baas:DescribeAntChain*"],

    "Effect": "Allow",

    "Resource": "acs:baas:*:*:*"

 },

 {

    "Action": "baas:*AntChainContract*",

    "Effect": "Allow",

    "Resource": ["acs:baas:*:*:antChainConsortium/$consortiumId/contractProject/$projectId"]

 }],

 "Version": "1"

}
```

