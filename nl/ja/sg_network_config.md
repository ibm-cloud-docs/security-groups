---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: configuration, network, virtual server, instance, security

subcollection: security-group


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# 既存のネットワーク構成とセキュリティー・グループ
{: #existing-network-configurations-and-security-groups}

セキュリティー・グループは既存のネットワーク構成を拡張します。 したがって、セキュリティー・グループは、相互に通信できないネットワーク間にまたがることはできません。
{: shortdesc}

仮想サーバー・インスタンスが相互に通信できない場合、それらをセキュリティー・グループに追加しても、その動作は変更されません。 ゲートウェイは、選択されたセキュリティー・グループによって定義されたトラフィックを許可する必要があります。

ご使用のアカウントで、カスタム・プライベート・アドレッシング (CPA) もセキュリティー・グループも有効になっている場合、セキュリティー・グループの適用範囲はアカウント・レベルであり、ネットワーク・レベルではないことに注意してください。 セキュリティー・グループは、プライベート・ネットワークではなく、IP アドレスによって定義されます。

セキュリティー・グループは、VSI のプロビジョニングを行うすべてのデータ・センターで使用できます。
