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

# 新規ルールの作成
{: #creating-a-new-rule}

以下の手順を実行して、入力要求 (SSH および ICMP) とその関連の (出力) トラフィック・フローを許可します。

1. [カスタマー・ポータル ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://cloud.ibm.com/classic){: new_window} の**「ルール」**タブを選択します。
2. **「ルールの作成」**をクリックします。
3. ルールの方向、IP タイプ、プロトコル、ポート範囲、タイプ、コード、およびソースを、(プロトコル選択に応じて) 該当する場合に指定します。

	別のセキュリティー・グループをソースとして使用していなければ、**「ソース・タイプ」**は「CIDR ブロック」のままにします。

	![ルールの作成](./images/rule_sg.jpg)

	この図では、**「すべての ICMP」**がプロトコルとして選択されています。つまり、すべての ICMP タイプおよびコードが許可されます。 さらに、「ソース」フィールドが空のままであるため、任意の IP アドレスまたはサブネットに相当するデフォルト値の `0.0.0.0/0` を使用します。

4. **「OK」**をクリックして終了します。

## 次のステップ...
{: #next-step-3}

セキュリティー・メニューまたはデバイス・メニューを使用して[セキュリティー・グループにインスタンスを割り当てます](/docs/infrastructure/security-groups?topic=security-groups-assigning-instances-to-the-security-group)。
