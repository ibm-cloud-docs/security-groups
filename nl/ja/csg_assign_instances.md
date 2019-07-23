---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"

keywords: assign, instance

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

# セキュリティー・グループへのインスタンスの割り当て
{: #assigning-instances-to-the-security-group}

セキュリティー・グループ・オブジェクトは、次の 2 つのいずれかの方法でインスタンスに割り当てることができます。

## セキュリティー・メニューの使用
{: #using-the-security-menu}

1. [カスタマー・ポータル ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://cloud.ibm.com/classic){: new_window} の**「セキュリティー」**タブで、**「ネットワーク・セキュリティー」**の下の**「セキュリティー・グループ」**を選択します。
2. インスタンスを割り当てるセキュリティー・グループ・オブジェクトの ![詳細アイコン](./images/more_icon.jpg) アイコンをクリックし、**「インスタンスの管理」**を選択します。
3. セキュリティー・グループに適用するインスタンスとインターフェースを選択します。

	![セキュリティー・メニューのインスタンス](./images/security_assign.jpg)

	この図では、セキュリティー・グループ「allow_icmp」 ([最初のステップ](/docs/infrastructure/security-groups?topic=security-groups-creating-a-security-group)で作成したもの) が、「jpmongevsi4」のプライベート・インターフェース (`10.0.2.219`) に適用されています。

	どのようにして**「接続されたインスタンス (Attached Instances)」**カウントが `0` から `1` に増えたかに注意してください。

4. **「保存」**をクリックして変更を適用します。

5. インスタンスをリブートします。

	これは、セキュリティー・グループで作成されなかったインスタンスのネットワーク・インターフェースごとに 1 回のみ実行するステップです。{: note}

## デバイス・メニューの使用
{: #using-the-devices-menu}

1. [カスタマー・ポータル ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://cloud.ibm.com/classic){: new_window} の**「デバイス」**タブから、**「デバイス・リスト」**を選択します。
2. セキュリティー・グループ・オブジェクトを適用するインスタンス名をクリックします。
3. **「変更」**を選択し、インスタンスに関連付けるセキュリティー・グループ・オブジェクトにマークを付けます。

	![デバイス・メニューのインスタンス](./images/device_assign.jpg)

	この図は、セキュリティー・グループ・オブジェクト「allow_icmp」が jpmongevsi4 インスタンスのプライベート・インターフェースに割り当てられることを示しています。
4. **「保存」**をクリックして変更を適用します。

5. インスタンスをリブートします。

	これは、セキュリティー・グループで作成されなかったインスタンスのネットワーク・インターフェースごとに 1 回のみ実行するステップです。{: note}

## 次のステップ...
{: #next-step-1}

[セキュリティー・グループを編集](/docs/infrastructure/security-groups?topic=security-groups-editing-a-security-group)し、そのパラメーターを変更します。  
