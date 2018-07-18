---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# 보안 그룹 API 참조
{: #api-reference} 

SoftLayer&reg; API(Application Programming Interface)는 개발자와 시스템 관리자가 SoftLayer 백엔드 시스템과 직접 상호작용하는
개발 인터페이스입니다. 
{:shortdesc}

SLAPI(SoftLayer API)는 고객 포털에 있는 기능의 대부분을 지원하므로
일반적으로 고객 포털에서 상호작용이 가능한 경우에는 API에서도 실행할 수 있습니다. API 내에서 SoftLayer 환경의 모든 부분과 프로그래밍 방식으로 상호작용할 수 있으므로 API를 사용하여 태스크를 자동화할 수 있습니다. 예를 들어, *SoftLayer_Virtual_Guest/createObject* API를 사용하여 보안 그룹이 사용으로 설정된 Virtual Server 인스턴스를 배치할 수 있습니다.

SoftLayer API는 원격 프로시저 호출(RPC) 시스템입니다. 각 호출에는 API 엔드포인트로 데이터를 전송하고 구조화된 데이터를 수신하는 과정이 포함됩니다. SLAPI를 통해 데이터를 전송하고 수신하는 데 사용되는 형식은 사용자가 선택한 API 구현에 따라 다릅니다. 

SoftLayer API, Virtual Server 및 보안 그룹 API에 대한 자세한 정보는 SoftLayer 개발 네트워크에서
다음 자원을 참조하십시오.
* [SoftLayer API 개요 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://sldn.softlayer.com/article/softlayer-api-overview){: new_window} 
* [SoftLayer API 시작하기 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](http://sldn.softlayer.com/article/getting-started){: new_window}
* [*SoftLayer_Virtual_Guest/createObject* API ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest/createObject){: new_window}
* [*SoftLayer_Network_SecurityGroup* API ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://sldn.softlayer.com/reference/services/SoftLayer_Network_SecurityGroup){: new_window}
* [*SoftLayer_Virtual_Guest_Network_Component* API ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest_Network_Component){: new_window}

SoftLayer API Python 클라이언트를 사용하여 보안 그룹과 상호작용할 수도 있습니다. 자세한 정보는 다음 링크를 참조하십시오.
* [SoftLayer API Python 클라이언트: Virtual Server에 대한 작업 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](http://softlayer-python.readthedocs.io/en/latest/cli/vs.html){: new_window}
* [softlayer_network_securitygroup에 대한 Python 예제 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://softlayer.github.io/classes/softlayer_network_securitygroup/){: new_window}
