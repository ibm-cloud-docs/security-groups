---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: create, new, rule, ssh, icmp

subcollection: security-group

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

# 创建新规则
{: #creating-a-new-rule}

通过执行以下过程来允许入局请求 (SSH & ICMP) 及其相关的（出局）流量：

1. 选择[客户门户网站 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://cloud.ibm.com/classic){: new_window} 的**规则**选项卡。
2. 单击**创建规则**。
3. 根据适用情况，指定规则的方向、IP 类型、协议、端口范围、类型、代码和源（基于协议的选择）。

	除非使用了其他安全组作为源，否则请保留**源类型**为“CIDR 块”。

	![创建规则](./images/rule_sg.jpg)

	此图显示选择为协议的**所有 ICMP**，这意味着将允许所有 ICMP 类型和代码。此外，“源”字段保留为空，使用缺省值 `0.0.0.0/0` -- 相当于任何 IP 地址或子网。

4. 单击**确定**以完成。

## 后续步骤...
{: #next-step-3}

使用安全菜单或设备菜单，[向安全组分配实例](/docs/infrastructure/security-groups?topic=security-groups-assigning-instances-to-the-security-group)。
