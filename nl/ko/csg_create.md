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

# 보안 그룹 작성
사용자 정의 보안 그룹을 작성하고 구성하십시오.

1. 브라우저에서 [고객 포털 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://control.softlayer.com/){: new_window}을 열고 사용자 계정에 로그인하십시오.
2.	**보안** 탭을 선택하십시오.
3. **네트워크 보안**에서 **보안 그룹**을 선택하십시오.
4.	**그룹 작성 +**을 클릭하십시오.
5.	보안 그룹 이름을 입력하고 선택적으로 설명을 입력하십시오.
6. **그룹 작성**을 클릭하십시오.

![보안 그룹 작성](./images/create_sg.jpg)

**기본값으로 그룹 작성…** 선택란이 선택 취소되었는지 확인하십시오. 이는 보안 그룹 오브젝트에 대해 아웃바운드 규칙이 작성되지 않는다는 의미입니다. 따라서 다른 아웃바운드 규칙 또는 보안 그룹 오브젝트가 작성되기 전까지는 수신 요청(예: SSH 및 ICMP) 및 이와 관련된 (발신) 트래픽 플로우나 응답만 허용됩니다.

## 다음 단계...
수신 요청(SSH & ICMP) 및 이와 관련된 (발신) 트래픽 플로우를 허용하는 [규칙을 작성](csg_rule.html)하십시오.  
