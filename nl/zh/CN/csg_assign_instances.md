---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"

keywords: assign, instance

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:note: .note}
{:important: .important}
{:tip: .tip}
{:table: .aria-labeledby="caption"}

# 向安全组分配实例
{: #assigning-instances-to-the-security-group}

您可以采用以下两种方式之一将安全组对象分配给实例：

## 使用安全菜单
{: #using-the-security-menu}

1. 从[客户门户网站 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://cloud.ibm.com/classic){: new_window} 的**安全**选项卡的**网络安全**下，选择**安全组**。
2. 单击想要向其分配实例的安全组对象的 ![“更多”图标](./images/more_icon.jpg) 图标，然后选择**管理实例**。
3. 选择要应用到安全组的实例和接口。

	![安全菜单实例](./images/security_assign.jpg)

	在图中，“allow_icmp”安全组（在[第一步](/docs/infrastructure/security-groups?topic=security-groups-creating-a-security-group)创建）应用到“jpmongevsi4”的专用接口 (`10.0.2.219`)。

	请注意**连接的实例数**计数如何从 `0` 增加到 `1`。

4. 单击**保存**以应用更改。

5. 重新引导实例。

	对于未使用安全组创建的实例的每个网络接口，只需执行此步骤一次。
  {: note}

## 使用设备菜单
{: #using-the-devices-menu}

1. 从[客户门户网站 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://cloud.ibm.com/classic){: new_window} 的**设备**选项卡上，选择**设备列表**。

2. 单击想要应用“安全组”对象的实例名称。
3. 选择**修改**，并标记想要与实例关联的安全组对象。

	![设备菜单实例](./images/device_assign.jpg)

	此图显示分配给 jpmongevsi4 实例的专用接口的“allow_icmp”安全组对象。
4. 单击**保存**以应用更改。

5. 重新引导实例。

	对于未使用安全组创建的实例的每个网络接口，只需执行此步骤一次。
  {: note}

## 后续步骤...
{: #next-step-1}

[编辑安全组](/docs/infrastructure/security-groups?topic=security-groups-editing-a-security-group)以修改其参数。  
