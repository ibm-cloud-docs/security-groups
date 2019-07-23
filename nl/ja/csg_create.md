---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: create, configure, configuration, custom

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:note: .note}
{:important: .important}
{:tip: .tip}
{:table: .aria-labeledby="caption"}

# セキュリティー・グループの作成
{: #creating-a-security-group}

以下のようにして、カスタム・セキュリティー・グループを作成して構成します。

1. ブラウザーから、[カスタマー・ポータル ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://cloud.ibm.com/classic){: new_window} を開き、アカウントにログインします。
2.	**「セキュリティー」**タブを選択します。
3. **「ネットワーク・セキュリティー」**から**「セキュリティー・グループ」**を選択します。
4.	**「グループの作成 +」**をクリックします。
5.	セキュリティー・グループの名前と、オプションで説明を入力します。
6. **「グループの作成」**をクリックします。

![セキュリティー・グループの作成](./images/create_sg.jpg)

**「すべてのアウトバウンド・トラフィックを許可するデフォルト・ルールを含むグループを作成する」**のチェック・ボックスにマークが付いていないことに注目してください。 これは、このセキュリティー・グループ・オブジェクトにアウトバウンド・ルールが作成されないことを意味します。 その結果、他のアウトバウンド・ルールまたはセキュリティー・グループ・オブジェクトが作成されなければ、入力要求 (SSH および ICMP など) とその関連の (出力) トラフィック・フローまたは応答のみが許可されます。

## 次のステップ...
{: #next-step-2}

入力要求 (SSH および ICMP) とその関連の (出力) トラフィック・フローを許可する[ルールを作成します](/docs/infrastructure/security-groups?topic=security-groups-creating-a-new-rule)。  
