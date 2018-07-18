---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 기존 네트워크 구성 및 보안 그룹

보안 그룹은 기존 네트워크 구성의 기능을 보강합니다. 따라서 보안 그룹은 서로 통신할 수 없는 네트워크 간에
확장될 수 없습니다. 
{:shortdesc}

Virtual Server 인스턴스가 서로 통신할 수 없는 경우 보안 그룹에 추가해도 해당 동작이 변경되지
않습니다. 게이트웨이가 선택한 보안 그룹에서 정의된 트래픽을 허용해야 합니다.

계정이 사용자 정의 사설 주소 지정(CPA) 및 보안 그룹에 대해 사용되는 경우 네트워크 레벨이 아니라 계정 레벨에서 보안 그룹의 범위가 지정됩니다. 보안 그룹은 사설 네트워크가 아니라 IP 주소별로 지정됩니다.

현재 다음 데이터 센터에서 보안 그룹을 사용할 수 있습니다.

|데이터 센터      | 
|:------------------|
| AMS01             |
| AMS03             |
|CHE01             |
| DAL01             |
| DAL05             |
| DAL06             |
| DAL09             |
| DAL10             |
|DAL12             |
|DAL13             |
| FRA02             |
| FRA04             |
| FRA05             |
|HKG02             |
| HOU02             |
| LON02             |
|LON04             |
| LON06             |
|MEL01             |
| MEX01             |
|MIL01             |
| MON01             |
|OSL01             |
| PAR01             |
|SAO01             |
| SEA01             |
| SEO01             |
| SJC01             |
| SJC03             |
|SJC04             |
| SNG01             |
|SYD01             |
|SYD04             |
| TOK02             |
|TOR01             |
| WDC01             |
| WDC04             |
|WDC06             |
|WDC07             |
{: caption="표 2. 보안 그룹을 지원하는 데이터 센터" caption-side="top"} 
