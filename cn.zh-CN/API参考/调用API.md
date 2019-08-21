# 调用API {#concept_1813825 .concept}

区块链服务API调用是通过向区块链服务的服务端地址发送HTTP请求。您需要并按照接口说明在请求中加入相应请求参数，调用后系统会返回处理结果。请求及返回结果都使用UTF-8字符集进行编码。

## 请求结构 {#section_8i8_hjn_umx .section}

区块链服务的API是RPC风格，您可以通过发送HTTP POST请求调用区块链服务。

其请求结构如下：

``` {#codeblock_ud1_btl_z1s}
http://Endpoint/?Action=xx&Parameters
```

其中：

-   Endpoint： 区块链服务API的服务接入地址为baas.aliyuncs.com。
-   Action：要执行的操作，如调用DescribeFabricOrganization接口查看已创建的服务实例。
-   Version：要使用的API版本，区块链服务的API版本是2018-12-21。
-   Parameters：请求参数，每个参数之间用“&”分隔。

    请求参数由公共请求参数和API自定义参数组成。公共参数中包含API版本号、身份验证等信息，详情请参见[公共参数](cn.zh-CN/API参考/公共参数.md#)。


下面是一个调用DescribeFabricOrganization接口查询已创建的区块链组织的示例：

**说明：** 为了便于用户查看，本文档中的示例都做了格式化处理。

``` {#codeblock_bln_7k1_ehl}
https://baas.aliyuncs.com/?Action=DescribeFabricOrganization
&Format=xml
&Version=2018-12-21
&Signature=xxxx%xxxx%3D
&SignatureMethod=HMAC-SHA1
&SignatureNonce=15215528852396
&SignatureVersion=1.0
&AccessKeyId=key-test
&Timestamp=2012-06-01T12:00:00Z
…
```

