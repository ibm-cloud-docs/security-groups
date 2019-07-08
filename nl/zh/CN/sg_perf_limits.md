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

# 安全组的性能限制
{: #performance-limitations-for-security-groups}

安全组及其关联的规则存在一些性能限制。
{: shortdesc}

|资源                                                  |限制                                               |
| --------------------------------------------------------- | --------------------------------------------------- |
|每个网络接口的安全组数                                    |5                                                   |
|每个帐户的安全组数                                        |500                                                 |
|每个安全组的规则数                                        |50                                                  |
|每个安全组的远程规则数                                    |5                                                   |
|每个安全组的网络接口数                                    |100                                                 |
{: caption="表 3. 特定资源的性能限制" caption-side="top"}

远程规则是将安全组指定为源或目标的规则。
{: note}
