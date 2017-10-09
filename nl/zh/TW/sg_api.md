---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Security Group API 參考資料
{: #api-reference} 

SoftLayer&reg; 應用程式設計介面 (API) 是開發介面，它可讓開發人員及系統管理者直接與 SoftLayer 的後端系統互動。
{:shortdesc}

SoftLayer API (SLAPI) 會啟動客戶入口網站中的許多特性，這通常表示如果可以在客戶入口網站中互動，便也可以在 API 執行。由於您可以透過程式設計方式，在 API 內與 SoftLayer 環境的所有部分互動，您可以使用 API 將作業自動化。例如，您可以使用 *SoftLayer_Virtual_Guest/createObject* API 來部署虛擬伺服器實例，並且啟用安全群組。

SoftLayer API 是「遠端程序呼叫」系統。每一個呼叫需要向 API 端點傳送資料，並反過來接收結構化資料。透過 SLAPI 傳送及接收資料時使用何種格式，視您選擇哪一個 API 實作而定。 

如需 SoftLayer API、虛擬伺服器及安全群組 API 的相關資訊，請參閱 SoftLayer Development Network 的下列資源：
* [SoftLayer API Overview ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://sldn.softlayer.com/article/softlayer-api-overview){: new_window} 
* [Getting Started with the SoftLayer API ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](http://sldn.softlayer.com/article/getting-started){: new_window}
* [*SoftLayer_Virtual_Guest/createObject* API ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest/createObject){: new_window}
* [*SoftLayer_Network_SecurityGroup* API ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://sldn.softlayer.com/reference/services/SoftLayer_Network_SecurityGroup){: new_window}
* [*SoftLayer_Virtual_Guest_Network_Component* API ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest_Network_Component){: new_window}

您也可以使用 SoftLayer API Python Client 與安全群組互動。如需相關資訊，請參閱下列鏈結：
* [SoftLayer API Python Client: Working with Virtual Servers ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](http://softlayer-python.readthedocs.io/en/latest/cli/vs.html){: new_window}
* [Python examples for softlayer_network_securitygroup ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://softlayer.github.io/classes/softlayer_network_securitygroup/){: new_window}
