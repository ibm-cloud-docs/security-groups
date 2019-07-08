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

# 安全群組的效能限制
{: #performance-limitations-for-security-groups}

安全群組及其相關聯規則有一些效能限制存在。
{: shortdesc}

|資源|限制|
| --------------------------------------------------------- | --------------------------------------------------- |
|每個網路介面的安全群組數|5                                                   |
|每個帳戶的安全群組數|500                                                 |
|每個安全群組的規則數|50                                                  |
|每個安全群組的遠端規則數|5                                                   |
|每個安全群組的網路介面數|100                                                 |
{: caption="表 3. 特定資源的效能限制" caption-side="top"}

遠端規則會指定安全群組作為來源或目的地。
{: note}
