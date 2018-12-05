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

# 建立安全群組
建立及配置自訂安全群組：

1. 從瀏覽器中，開啟[客戶入口網站 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){: new_window}，並登入您的帳戶。
2.	選取**安全**標籤。
3. 從**網路安全**中選取**安全群組**。
4.	按一下**建立群組 +**。
5.	輸入「安全群組」的名稱，及選擇性地輸入說明。
6. 按一下**建立群組**。

![建立安全群組](./images/create_sg.jpg)

請注意，**建立含有預設值的群組…** 勾選框已取消勾選。這表示將不會針對此「安全群組」物件建立出埠規則。因此，除非建立其他出埠規則或「安全群組」物件，否則，僅允許送入的要求（例如 SSH 及 ICMP）及其相關的（送出的）資料傳輸流或回應。

## 下一步...
[建立規則](csg_rule.html)，以容許送入的要求 (SSH & ICMP) 及其相關的（送出的）資料傳輸流。  
