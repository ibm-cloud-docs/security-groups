---



copyright:
  years: 2017
lastupdated: "2018-11-10"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# 创建安全组
创建和配置定制安全组：

1. 从浏览器，打开[客户门户网站 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){: new_window}，并登录到帐户。
2.	选择**安全**选项卡。
3. 从**网络安全**，选择**安全组**。
4.	单击**创建组 +**。
5.	输入安全组的名称以及（可选）描述。
6. 单击**创建组**。

![创建安全组](./images/create_sg.jpg)

请注意，**使用缺省值创建组…** 复选框处于取消选中状态。这意味着不会为此安全组对象创建出站规则。因此，除非创建其他出站规则或安全组对象，否则将只允许入局请求（例如 SSH 和 ICMP）及其相关的（出局）流量或响应。

## 后续步骤...
[创建规则](csg_rule.html)以允许入局请求 (SSH & ICMP) 及其相关的（出局）流量。  
