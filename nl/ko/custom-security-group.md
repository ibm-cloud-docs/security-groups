---



copyright:
  years: 2017
lastupdated: "2018-11-10"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# 사용자 정의 보안 그룹 작성 및 관리
{: #creating-and-managing-a-custom-security-group}

이 튜토리얼에서 사용자 정의 보안 그룹을 작성하고 보안 그룹에 인스턴스를 지정하며 보안 그룹을 편집하는 방법을 알아봅니다.

![사용자 정의 보안 그룹](./images/goal.jpg)

## 필요한 항목
이 예제에서는 다음 오브젝트와 항목이 사용됩니다.

| 리소스 이름  | 운영 체제 |유형 | 위치/DC | IP/서브넷 |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| 해당되지 않음/임의 | 10.0.0.0/16 |
| allow_icmp | 해당되지 않음  | 보안 그룹 | 해당되지 않음/임의 | 0.0.0.0/0 |
| allow_ssh | 해당되지 않음 | 보안 그룹 | 해당되지 않음/임의 | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Virtual Server 인스턴스 | Dallas 10 Pod 01 | 10.0.0.21 |
|jpmongevsi4.testing.com | Ubuntu 16.04 | Virtual Server 인스턴스 |	Dallas 10 Pod 01	| 10.0.2.219 |


이 튜토리얼에서는 CPA 사설 네트워크/계정을 사용하지만 사실상 보안 그룹은 CPA 계정과 일반 계정에서 동일한 방식으로 작동합니다. 서브넷 10.0.0.0/24 및 10.0.2.0/24는 동일한 CPA 사설 네트워크에 속하며, 이는 동일한 사설 서브넷/VLAN에 두 개 이상의 VSI가 연결된 일반 계정을 가지는 것과 동일합니다.


## 수행할 작업

이 튜토리얼에서는 다음을 수행할 방법에 대해 알아봅니다.

태스크  |설명
------------- | -------------
[보안 그룹 작성](/docs/infrastructure/security-groups?topic=security-groups-creating-a-security-group) | IBM© 클라우드 플랫폼에서 사전 정의된 항목을 사용하는 것과는 대조적으로 사용자 정의 보안 그룹을 작성하고 구성합니다. 
[규칙 작성](/docs/infrastructure/security-groups?topic=security-groups-creating-a-new-rule) | 수신 요청(SSH & ICMP) 및 이와 관련된 (발신) 트래픽 플로우를 허용하는 규칙을 작성합니다.
[보안 그룹에 인스턴스 지정](/docs/infrastructure/security-groups?topic=security-groups-assigning-instances-to-the-security-group) | 보안 메뉴 또는 디바이스 메뉴를 사용하여 인스턴스에 보안 그룹 오브젝트를 지정합니다.
[보안 그룹 및 규칙 편집](/docs/infrastructure/security-groups?topic=security-groups-editing-a-security-group) | 보안 오브젝트 및 해당 규칙에 대한 매개변수를 수정합니다.
