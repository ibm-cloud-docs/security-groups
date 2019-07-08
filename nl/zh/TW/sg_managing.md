---



copyright:
  years: 2017, 2019
lastupdated: "2019-06-11"

keywords: manage, details, edit, configure

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# 管理安全群組
{: #managing-sg}

您可以使用 {{site.data.keyword.cloud}} 基礎架構客戶入口網站的「安全群組」頁面或「裝置詳細資料」頁面來管理安全群組。
{: shortdesc}

## 從安全群組頁面管理安全群組
{: #managing-security-groups-from-security-groups-page}

若要從「安全群組」頁面管理安全群組，請完成下列步驟：


1. 從[客戶入口網站 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/) 導覽，選取**安全 -> 網路安全 -> 安全群組**。
2. 在「安全群組」區段下，您可以完成數個管理作業。
     * 檢視安全群組的清單。
     * 建立群組。
     * 編輯群組資訊。
     * 複製群組。
     * 刪除群組。

## 從安全群組頁面管理安全群組規則
{: #managing-security-group-rules-from-security-groups-page}

若要從「安全群組」頁面管理安全群組規則，請完成下列步驟：


1. 從[客戶入口網站 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/) 導覽，選取**安全 -> 網路安全 -> 安全群組**。
2. 按一下安全群組名稱以開啟「詳細資料」頁面。
3. 從「安全群組詳細資料」頁面，您可以完成數個管理作業。
     * 檢視針對安全群組定義的規則清單。
     * 建立新的規則。
     * 編輯規則。
     * 刪除規則。
     * 檢視虛擬伺服器實例及指派給安全群組的相關聯介面。

如果您刪除安全群組中的最後一個規則，則此安全群組將不容許任何入埠或出埠資料流量。
{: tip}

## 從裝置詳細資料頁面管理安全群組
{: #managing-security-groups-from-device-details-page}

若要從「裝置詳細資料」頁面管理安全群組，請完成下列步驟：


1. 從[客戶入口網站 ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/)，選取**裝置 -> 裝置清單**。
2. 選取您訂購的虛擬伺服器的裝置名稱。即會開啟「裝置詳細資料」頁面。
3. 從「裝置詳細資料」頁面，驗證您是否已在**配置**標籤。
4. 在「安全群組」區段下，您可以完成數個管理作業。
     * 檢視安全群組及規則。
     * 將安全群組指派給虛擬伺服器實例的網路介面。
     * 將安全群組從虛擬伺服器實例的網路介面移除。

     在您第一次指派現有安全群組給網路介面（公用或專用）時，必須重新啟動每個介面。不過，如果同時指派公用及專用介面給安全群組，則只需要重新啟動一次。重新啟動之後，會自動套用變更。
     {: important}

     當您指派新的安全群組時，會根據安全群組規則定義而防止建立新連線。不過，並不會終止現有的 Socket 連線。

     如果您移除指派給虛擬伺服器實例的最後一個安全群組，則虛擬伺服器資料流量不再受到安全群組的限制。安全群組防火牆不再存在。
     {: tip}

6. 完成變更之後，請按一下**儲存**。
