---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: performance, limits, limitations, rules

subcollection: security-group


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# セキュリティー・グループのパフォーマンス上の制限
{: #performance-limitations-for-security-groups}

セキュリティー・グループとその関連ルールには、パフォーマンス上の制限がいくつかあります。
{: shortdesc}

| リソース                                                  | 制限                                               |
| --------------------------------------------------------- | --------------------------------------------------- |
| ネットワーク・インターフェース当たりのセキュリティー・グループ数                     | 5                                                   |
| アカウント当たりのセキュリティー・グループ数                               | 500                                                 |
| セキュリティー・グループ当たりのルール数                                  | 50                                                  |
| セキュリティー・グループ当たりのリモート・ルール数                           | 5                                                   |
| セキュリティー・グループ当たりのネットワーク・インターフェース数                     | 100                                                  |
{: caption="表 3. 特定のリソースのパフォーマンス上の制限" caption-side="top"}

リモート・ルールとは、セキュリティー・グループをソースまたは宛先として指定するルールを指します。
{: note}
