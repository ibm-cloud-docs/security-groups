---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 現有的網路配置及安全群組

安全群組會擴增任何現有的網路配置。因此，安全群組不能跨越無法彼此通訊的網路。
{:shortdesc}

如果虛擬伺服器實例無法彼此通訊，將它們新增至安全群組並不會變更該行為。閘道必須容許所選安全群組定義的資料流量。

如果您的帳戶已啟用自訂專用定址 (CPA) 以及安全群組，請注意，安全群組的範圍限定在帳戶層次，而非網路層次。安全群組由 IP 位址所定義，而非專用網路。

安全群組目前可用於下列資料中心：

|資料中心| 
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
{: caption="表 2. 支援安全群組的資料中心" caption-side="top"} 
