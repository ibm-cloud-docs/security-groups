---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"

keywords: add, order, group

subcollection: security-groups


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# 订购期间添加预定义的安全组
{: #adding-a-pre-defined-security-group-during-ordering}

此分步过程向您显示如何在订购期间向实例添加现有或预定义安全组。

您可以使用“安全组”来制定一组 IP 过滤器规则，这些规则用于定义如何处理通过虚拟服务器实例的公共和专用接口的入局和出局流量。


![定制安全组](./images/goal2.jpg)

## 所需内容
{: #what-you-ll-need-2}

对于此示例，将使用以下对象和项目：

| 资源名称|操作系统|类型| 位置/DC | IP/子网|
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| allow_ssh1 |不适用|安全组| 不适用/任意| 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | 虚拟服务器实例| Dallas 10 Pod 01 | 10.0.0.21 |
|jpmongevsi4.testing.com | Ubuntu 16.04 | 虚拟服务器实例|	Dallas 10 Pod 01	| 10.0.2.219 |

## 订购安全组
{: #order-a-security-group}

要订购虚拟服务器实例并分配安全组，请执行以下过程：

1. 从浏览器打开[客户门户网站 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/)，然后登录帐户。
2. 找到**订单**部分，然后单击**设备**。
3. 在“设备”页面上，单击某个虚拟服务器产品的**按小时**或**按月**。
4. 在“配置云服务器”订单页面上，必须选择支持安全组的数据中心。
5. 完成其他所需信息，然后单击**添加到订单**。此时将打开“结帐”页面。
6. 确认以下 VSI 信息：

	* 位置
	* 规范
	* 网络端口选项。

7. 从**配置安全组**，选择想要应用的安全组。可以通过单击**查看规则**链接来显示每个安全组的关联规则。

	![定制安全组](./images/sgs.jpg)

	您可以选择将任意预定义的安全组应用于虚拟服务器上的专用或公共接口。

8. 指定实例名称。
9. 标记云服务术语和第三方服务协议复选框（如果适用）。
10. 最后，单击**提交订单**。
