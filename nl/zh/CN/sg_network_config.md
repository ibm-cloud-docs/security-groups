---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 现有网络配置和安全组

安全组可以作为任何现有网络配置的补充。因此，安全组无法跨越不能彼此通信的网络。
{:shortdesc}

如果虚拟服务器实例之间不能彼此通信，那么即使将其添加到安全组也不会改变其行为。网关必须允许由所选安全组定义的流量。

如果帐户已启用定制私有寻址 (CPA) 和安全组，那么请注意安全组的作用域是帐户级别，而不是网络级别。安全组是按 IP 地址而不是专用网络定义的。

安全组当前在以下数据中心可用：

|数据中心      | 
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
{: caption="表 2. 支持安全组的数据中心" caption-side="top"} 
