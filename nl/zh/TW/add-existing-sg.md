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

# 在訂購期間新增預先定義的安全群組
{: #adding-a-pre-defined-security-group-during-ordering}

此逐步程序顯示如何在訂購處理程序期間，將現有的或預先定義的安全群組新增至實例。

您可以使用「安全群組」來制定一組 IP 過濾器規則，定義如何處理對虛擬伺服器實例之公用和專用介面的送入及送出資料流量。


![自訂安全群組](./images/goal2.jpg)

## 需要的項目
{: #what-you-ll-need-2}

以本範例而言，將使用下列物件及項目：

| 資源名稱       | 作業系統         | 類型 | 位置/DC     | IP/子網路 |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| allow_ssh1 | 不適用          | 安全群組       | 不適用/任何        | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | 虛擬伺服器實例          |Dallas 10 Pod 01	| 10.0.0.21 |
|jpmongevsi4.testing.com | Ubuntu 16.04 | 虛擬伺服器實例          |	Dallas 10 Pod 01	| 10.0.2.219 |

## 訂購安全群組
{: #order-a-security-group}

若要訂購虛擬伺服器實例及指派安全群組，請執行下列程序：

1. 從您的瀏覽器開啟[客戶入口網站 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/) 然後登入您的帳戶。
2. 找到**訂購**區段，並按一下**裝置**。
3. 在「裝置」頁面上，針對其中一個虛擬伺服器供應項目按一下**每小時**或**每月**。
4. 在「配置雲端伺服器訂單」頁面上，您必須選取支援安全群組的資料中心。
5. 完成任何其他必要資訊，並按一下**新增至訂單**。即會開啟「結帳」頁面。
6. 確認 VSI 的下列資訊：

	* 位置
	* 規格
	* 網路埠選項。

7. 從**配置安全群組**中，選取想要套用的「安全群組」。可按一下**檢視規則**鏈結來顯示每一個「安全群組」的關聯規則。

	![自訂安全群組](./images/sgs.jpg)

	您可以選取任何預先定義的安全群組，以套用至虛擬伺服器上的專用或公用介面。

8. 指定實例名稱。
9. 在適當的情況下，勾選「雲端服務」條款及「協力廠商服務合約」勾選框。
10. 最後，按一下**提交訂單**。
