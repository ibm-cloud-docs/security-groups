---

copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: create, rules, assign, interface, virtual server

subcollection: security-group
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}


# 创建安全组和规则
{: #creating-security-groups}

您可以创建安全组及其关联的规则，然后将其分配给一个或多个虚拟服务器实例的接口以启用虚拟防火墙。


## 创建安全组
{: #creating-a-security-group-1}

要创建安全组，请完成以下步骤：


1. 在[客户门户网站 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/) 导航中，选择**安全性 -> 网络安全性 -> 安全组**。
2. 在“安全组”页面中，单击**创建组**。
3. 输入安全组的名称和描述，然后再次单击**创建组**。

缺省情况下选择了**使用缺省规则创建组以允许所有出站流量**。您可以清除此字段，以创建没有规则的安全组。没有规则的安全组会阻止所有流量（入站和出站）。
{: note}

## 创建安全组规则
{: #creating-security-group-rules}

要创建安全组规则，请完成以下步骤：


1. 在[客户门户网站 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/) 导航中，选择**安全性 > 网络安全性 > 安全组**。
2. 在“安全组”页面中，单击安全组名称以打开“详细信息”页面，并选择**创建规则**。
3. 在“创建规则”页面中，输入所有相应的属性（如方向、IP 类型、协议和源/目标信息）。完成后，单击**确定**。

选择可选的源或目标字段将限制新规则，使其仅适用于流入/流出指定源/目标的流量。源和目标字段可以指定无类域间路由 (CIDR) 块或安全组。
{: note}

CIDR 块有助于 IP 地址块的路由。如果选择 CIDR 类型，那么必须指定 IP 地址范围。

如果选择安全组类型，那么必须从现有安全组列表中进行选择。此选择可以是连接到所选安全组的设备的任意 IP 地址。如果虚拟服务器配置为具有多个 IP 地址，那么这些远程安全组规则只会使用主 IPv4 和 IPv6 地址。
