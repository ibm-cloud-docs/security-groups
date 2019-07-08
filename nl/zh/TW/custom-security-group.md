---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: create, manage, custom, instance, assign, edit

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

# 建立及管理自訂安全群組
{: #creating-and-managing-a-custom-security-group}

在本指導教學中，您將學會如何建立、指派實例及編輯自訂「安全群組」。

![自訂安全群組](./images/goal.jpg)

## 需要的項目
{: #what-you-ll-need-3}

以本範例而言，將使用下列物件及項目：

| 資源名稱       | 作業系統         | 類型 | 位置/DC     | IP/子網路 |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| 不適用/任何        | 10.0.0.0/16 |
| allow_icmp | 不適用          | 安全群組       | 不適用/任何        | 0.0.0.0/0 |
| allow_ssh | 不適用          | 安全群組       | 不適用/任何        | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | 虛擬伺服器實例          |Dallas 10 Pod 01	| 10.0.0.21 |
|jpmongevsi4.testing.com | Ubuntu 16.04 | 虛擬伺服器實例          |	Dallas 10 Pod 01	| 10.0.2.219 |


請注意，本指導教學是利用 CPA 專用網路/帳戶，不過，在實際用途上，「安全群組」在 CPA 帳戶及一般帳戶中的行為方式相同。子網路 10.0.0.0/24 及 10.0.2.0/24 屬於相同的 CPA 專用網路，這相當於一般帳戶有兩個以上的 VSI 連接到相同的專用子網路/VLAN。


## 您將達成的目標
{: #what-you-ll-accomplish-3}

在本指導教學中，您將學會如何...

作業  |說明
------------- | -------------
[建立安全群組](/docs/infrastructure/security-groups?topic=security-groups-creating-a-security-group) | 建立及配置自訂安全群組，相對於使用 IBM© Cloud 平台預先定義的安全群組。
[建立規則](/docs/infrastructure/security-groups?topic=security-groups-creating-a-new-rule)  | 建立規則，以容許送入的要求 (SSH & ICMP) 及其相關的（送出的）資料傳輸流。
[將實例指派給「安全群組」](/docs/infrastructure/security-groups?topic=security-groups-assigning-instances-to-the-security-group) | 使用「安全功能表」或「裝置功能表」，將「安全群組」物件指派給實例。
[編輯安全群組及其規則](/docs/infrastructure/security-groups?topic=security-groups-editing-a-security-group) | 修改「安全物件」的參數及其規則。
