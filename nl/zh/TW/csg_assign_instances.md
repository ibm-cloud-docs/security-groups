---



copyright:
  years: 2017, 2018
lastupdated: "2018-02-15"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# 指派安全群組的實例
您有兩種方式可將安全群組物件指派到實例中：

## 使用安全功能表

1. 從[客戶入口網站 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){: new_window}上的**安全**標籤，選取**網路安全**之下的**安全群組**。
2. 按一下您要對其指派實例的「安全群組」物件的![其他圖示](./images/more_icon.jpg)圖示，然後選取**管理實例**。
3. 選取要套用至「安全群組」的實例及介面。

	![安全功能表實例](./images/security_assign.jpg)

	在此圖中，"allow_icmp" 安全群組（在[首要步驟](csg_create.html)中所建立）已套用至 "jpmongevsi4" 的專用介面 (`10.0.2.219`)。

	請注意，**附加的實例**計數如何從 `0` 增加為 `1`。

4. 按一下**儲存**，即可套用變更。

5. 重新啟動實例。

	**附註：**這是針對建立時不具備安全群組的實例所進行，每個網路介面的一次性步驟。

## 使用裝置功能表

1. 從[客戶入口網站 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){: new_window}上的**裝置**標籤，選取**裝置清單**。
2. 按一下您要在其中套用「安全群組」物件的實例名稱。
3. 選取**修改**，並標示您想要與實例相關聯的「安全群組」物件。

	![裝置功能表實例](./images/device_assign.jpg)

	此圖顯示將 "allow_icmp" 這個「安全群組」物件指派給 jpmongevsi4 實例的專用介面。
4. 按一下**儲存**，即可套用變更。

5. 重新啟動實例。

	**附註：**這是針對建立時不具備安全群組的實例所進行，每個網路介面的一次性步驟。

## 下一步...
[編輯安全群組](csg_edit.html)以修改其參數。  
