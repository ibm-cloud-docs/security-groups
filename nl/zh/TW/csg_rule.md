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

# 建立新規則
{: #creating-a-new-rule}

執行下列程序，以容許送入的要求 (SSH & ICMP) 及其相關的（送出的）資料傳輸流：

1. 選取[客戶入口網站 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://cloud.ibm.com/classic){: new_window}上的**規則**標籤。
2. 按一下**建立規則**。
3. 在適當的情況下，指定規則的「方向」、「IP 類型」、「通訊協定」、「埠範圍」、「類型」、「程式碼」及「來源」（根據「通訊協定」選擇）。

	除非您使用另一個「安全群組」作為來源，否則請保留**來源類型**為「CIDR 區塊」。

	![建立規則](./images/rule_sg.jpg)

	此圖顯示已選取**所有 ICMP** 作為通訊協定，這表示將容許所有 ICMP 類型及程式碼。此外，「來源」欄位保留空白，而使用預設值 `0.0.0.0/0` -- 相當於任何 IP 位址或子網路。

4. 按一下**確定**以完成。

## 下一步...
{: #next-step-3}

使用「安全功能表」或「裝置功能表」，[將實例指派給「安全群組」](/docs/infrastructure/security-groups?topic=security-groups-assigning-instances-to-the-security-group)。
