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

# Kubernetes의 확장 가능한 웹 앱
다음 프로시저를 수행하여 수신 요청(SSH & ICMP) 및 이와 관련된 (발신) 트래픽 플로우를 허용하십시오.

1. [고객 포털 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://cloud.ibm.com/classic){: new_window}에서 **규칙** 탭을 선택하십시오.
2.	**규칙 작성**을 클릭하십시오.
3.	해당되는 경우(프로토콜 선택사항에 따라) 규칙의 방향, IP 유형, 프로토콜, 포트 범위, 유형, 코드 및 소스를 지정하십시오. 

	다른 보안 규칙을 소스로 사용하지 않는 한, **소스 유형**을 "CIDR 블록"으로 두십시오.
	
	![규칙 작성](rule_sg.jpg)
	
	이 그림에서는 프로토콜로 선택된 **모든 ICMP**를 보여주며, 이는 모든 ICMP 유형과 코드가 허용된다는 것을 의미합니다. 또한 소스 필드는 기본값 `0.0.0.0/0`을 사용하여 비어 있는 상태입니다(모든 IP 주소 또는 서브넷에 동일함).

4.	**확인**을 클릭하여 완료하십시오.
