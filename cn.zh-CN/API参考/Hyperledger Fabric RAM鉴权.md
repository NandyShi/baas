# Hyperledger Fabric RAM鉴权 {#concept_1375180 .concept}

在使用RAM账号调用区块链服务API前，需要主账号通过创建授权策略对RAM账号进行授权。在授权策略中，使用资源描述符（Alibaba Cloud Resource Name，ARN）指定授权资源。

本文提供了在区块链服务中通过访问控制实现团队或者部门成员鉴权、跨账号资源授权以及跨云服务授权的RAM鉴权规则。在了解如何使用访问控制RAM授权和访问区块链服务之前，确保您已阅读了[RAM产品文档](https://help.aliyun.com/document_detail/28627.html#concept-oyr-zzv-tdb)和[RAM API文档](https://help.aliyun.com/document_detail/62184.html#concept-vdd-rmk-xdb)。

## 可授权的Hyperledger Fabric资源类型 {#section_v36_qb8_5m4 .section}

在进行RAM子账号授权时，Hyperledger Fabric资源的描述方式如下：

|资源类型|授权策略中的资源描述方法|
|----|------------|
|联盟|acs:baas:$regionId:$accountId:consortium/$consortiumId|
|组织|acs:baas:$regionId:$accountId:organization/$organizationId|
|通道|acs:baas:\*:$accountId:channel/$channelId|
|链码|acs:baas:\*:$accountId:chaincode/$chiancodeId|

其中，`$regionId`为具体资源所在的region。`$accountId`为具体资源属主的阿里云云账号Id。`$consortiumId/$organizationId/$channelId/$chiancodeId`为具体资源在区块链服务中的资源Id。

**说明：** 通道和链码属于全局资源，region必须为“\*”。

## 可授权的Hyperledger Fabric接口 {#section_jmn_qp9_ro8 .section}

下表列举了Hyperledger Fabric区块链中默认授权的API（子账号以及STS Token持有者默认拥有权限）：

|API|
|---|
|CheckFabricConsortiumDomain|
|CheckFabricOrganizationDomain|
|DescribeTasks|
|DescribeRootDomain|
|DescribeFabricConsortiumConfig|
|DescribeFabricConsortiumSpecs|
|DescribeFabricOrganizationSpecs|
|DescribeFabricInviter|
|DescribeFabricChaincodeUploadPolicy|
|AcceptFabricInvitation|

下表列举了Hyperledger Fabric中可授权的API及其描述方式：

|API|资源描述|
|---|----|
|CreateFabricOrganization|acs:baas:$regionId:$accountId:organization/\*|
|DescribeFabricOrganization|acs:baas:$regionId:$accountId:organization/$organizationId|
|DescribeFabricOrganizationDeletable|acs:baas:$regionId:$accountId:organization/$organizationId|
|DescribeFabricOrganizations|acs:baas:\*:$accountId:organization/\*|
|DescribeFabricCandidateOrganizations|acs:baas:\*:$accountId:organization/\*|
|CreateFabricChannel|acs:baas:\*:$accountId:channel/\* acs:baas:$regionId:$accountId:consortium/$consortiumId

 |
|DescribeFabricOrganizationChannels|acs:baas:$regionId:$accountId:organization/$organizationId|
|DescribeFabricConsortiumChannels|acs:baas:$regionId:$accountId:consortium/$consortiumId|
|CreateFabricChannelMember|acs:baas:\*:$accountId:channel/$channelId|
|DescribeFabricChannelMembers|acs:baas:\*:$accountId:channel/$channelId|
|JoinFabricChannel|acs:baas:\*:$accountId:channel/$channelId|
|CreateFabricConsortium|acs:baas:$regionId:$accountId:consortium/\*|
|CreateFabricConsortiumMember|acs:baas:$regionId:$accountId:consortium/$consortiumId|
|ConfirmFabricConsortiumMember|acs:baas:$regionId:$accountId:consortium/$consortiumId|
|DescribeFabricOrganizationMembers|acs:baas:$regionId:$accountId:organization/$organizationId|
|DescribeFabricOrganizationPeers|acs:baas:$regionId:$accountId:organization/$organizationId|
|DescribeFabricConsortiums|acs:baas:\*:$accountId:consortium/\*|
|DescribeFabricConsortiumAdminStatus|acs:baas:\*:$accountId:consortium/\*|
|DescribeFabricConsortiumMembers|acs:baas:$regionId:$accountId:consortium/$consortiumId|
|DescribeFabricConsortiumMemberApproval|acs:baas:$regionId:$accountId:consortium/$consortiumId|
|DescribeFabricConsortiumOrderers|acs:baas:$regionId:$accountId:consortium/$consortiumId|
|DescribeFabricConsortiumDeletable|acs:baas:$regionId:$accountId:consortium/$consortiumId|
|CreateFabricChaincode|acs:baas:\*:$accountId:chaincode/\* acs:baas:\*:$accountId:channel/$channelId

 acs:baas:$regionId:$accountId:consortium/$consortiumId

 acs:baas:$regionId:$accountId:organization/$organizationId

 |
|DescribeFabricOrganizationChaincodes|acs:baas:$regionId:$accountId:organization/$organizationId|
|DescribeFabricConsortiumChaincodes|acs:baas:$regionId:$accountId:consortium/$consortiumId|
|DeleteFabricChaincode|acs:baas:\*:$accountId:chaincode/$chaincodeId|
|InstallFabricChaincode|acs:baas:\*:$accountId:chaincode/$chaincodeId acs:baas:$regionId:$accountId:organization/$organizationId

 |
|InstantiateFabricChaincode|acs:baas:\*:$accountId:chaincode/$chaincodeId acs:baas:$regionId:$accountId:organization/$organizationId

 |
|UpgradeFabricChaincode|acs:baas:\*:$accountId:chaincode/$chaincodeId acs:baas:$regionId:$accountId:organization/$organizationId

 |
|SynchronizeFabricChaincode|acs:baas:\*:$accountId:chaincode/$chaincodeId acs:baas:$regionId:$accountId:organization/$organizationId

 |
|CreateFabricOrganizationUser|acs:baas:$regionId:$accountId:organization/$organizationId|
|DescribeFabricOrganizationUsers|acs:baas:$regionId:$accountId:organization/$organizationId|
|ResetFabricOrganizationUserPassword|acs:baas:$regionId:$accountId:organization/$organizationId|
|DownloadFabricOrganizationSDK|acs:baas:$regionId:$accountId:organization/$organizationId|
|DescribeFabricInvitationCode|acs:baas:$regionId:$accountId:consortium/$consortiumId|

## Hyperledger Fabric RAM规则示例 {#section_ko0_gzr_w3r .section}

例1 ：授权BaaS服务只读类操作。这种类型的权限能够允许用户通过控制台或API查看区块链状态，下载SDK。

``` {#codeblock_1ns_hgc_4iv}
{
   "Statement": [{ 
       "Action": ["baas:Describe*","baas:DownloadFabricOrganizationSDK"],
       "Effect": "Allow",
       "Resource": "acs:baas:*:*:*"
   }],
   "Version": "1"
}
```

例2：授权链码管理类操作（上传、安装、实例化等等）。这种类型的权限允许用户通过控制台或API管理所有链码。

``` {#codeblock_qnk_ewq_3hz}
{
  "Statement": [{
     "Action": "baas:*Chaincode",
     "Effect": "Allow",
     "Resource": ["acs:baas:*:*:chaincode/*","acs:baas:*:*:organization/*", "acs:baas:*:*:consortium/*","acs:baas:*:*:channel/*"]
  }],
  "Version": "1"
}
```

例3：更精细化的链码开发者授权。该权限通常需要全部的读类型操作，以及特定组织的链码管理类操作。按照最小权限原则，需要限制该用户仅能创建用于指定联盟、组织、通道的链码，也只能在特定组织上进行链码的安装、实例化等操作。将下面的`$consortiumId/$organizationId/$channelId`替换为具体资源在区块链服务中的资源Id。

``` {#codeblock_rly_ikp_fgk}
{
 "Statement": [{
   "Action": ["baas:Describe*","baas:DownloadFabricOrganizationSDK"],
   "Effect": "Allow",
   "Resource": "acs:baas:*:*:*"
 },
 {
   "Action": "baas:*Chaincode",
   "Effect": "Allow",
   "Resource": ["acs:baas:*:*:chaincode/*","acs:baas:*:*:organization/$organizationId","acs:baas:*:*:consortium/$consortiumId","acs:baas:*:*:channel/$channelId"]
 }],
 "Version": "1"
}
```

