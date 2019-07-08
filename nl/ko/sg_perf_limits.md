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

# 보안 그룹의 성능 제한사항
{: #performance-limitations-for-security-groups}

보안 그룹 및 연관된 규칙에 대한 몇 가지 성능 제한사항이 있습니다.
{: shortdesc}

|리소스                                                  |한계                                               |
| --------------------------------------------------------- | --------------------------------------------------- |
|네트워크 인터페이스당 보안 그룹                     |5                                                   |
|계정당 보안 그룹                               |500                                                 |
|보안 그룹당 규칙                                  |50                                                  |
|보안 그룹당 원격 규칙                           |5                                                   |
|보안 그룹당 네트워크 인터페이스                     |100                                                  |
{: caption="표 3. 특정 리소스에 대한 성능 제한사항" caption-side="top"}

원격 규칙은 보안 그룹을 소스 또는 대상으로 지정하는 규칙입니다.
{: note}
