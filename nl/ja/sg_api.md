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

# セキュリティー・グループ API リファレンス
{: #api-reference} 

SoftLayer® アプリケーション・プログラミング・インターフェース (API) は、開発者やシステム管理者が SoftLayer のバックエンド・システムと直接対話できるようにする開発用インターフェースです。 
{:shortdesc}

SoftLayer API (SLAPI) は、カスタマー・ポータルの多くの機能を備えています。つまり、一般に、カスタマー・ポータルで可能な対話を API でも実行できます。 API 内で SoftLayer 環境のすべての部分とプログラムで対話できるので、API を使用してタスクを自動化できます。 例えば、*SoftLayer_Virtual_Guest/createObject* API を使用して、セキュリティー・グループを有効にした仮想サーバー・インスタンスをデプロイできます。

SoftLayer API は、リモート・プロシージャー・コール・システムです。 各呼び出しでは、API エンドポイントにデータを送信し、戻りとして構造化データを受け取ります。 SLAPI でのデータの送信と受信に使用される形式は、選択した API の実装方法によって異なります。 

SoftLayer API、仮想サーバー、およびセキュリティー・グループ API について詳しくは、SoftLayer Development Network にある以下のリソースを参照してください。
* [SoftLayer API Overview ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://softlayer.github.io/reference/softlayerapi/){: new_window} 
* [Getting Started with the SoftLayer API ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](http://sldn.softlayer.com/article/getting-started){: new_window}
* [*SoftLayer_Virtual_Guest/createObject* API ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest/createObject){: new_window}
* [*SoftLayer_Network_SecurityGroup* API ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://sldn.softlayer.com/reference/services/SoftLayer_Network_SecurityGroup){: new_window}
* [*SoftLayer_Virtual_Guest_Network_Component* API ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest_Network_Component){: new_window}

SoftLayer API Python Client を使用して、セキュリティー・グループと対話することもできます。 詳しくは、以下のリンクを参照してください。
* [SoftLayer API Python Client: Working with Virtual Servers ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](http://softlayer-python.readthedocs.io/en/latest/cli/vs.html){: new_window}
* [Python の softlayer_network_securitygroup の例 ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://softlayer.github.io/classes/softlayer_network_securitygroup/){: new_window}
