---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Configurations réseau existantes et groupes de sécurité

Un groupe de sécurité permet d'étendre une configuration réseau existante. Par conséquent, un groupe de sécurité ne peut pas être étendu sur des réseaux incapables de pas communiquer entre eux. 
{:shortdesc}

Si des instances de serveur virtuel ne parviennent pas à communiquer entre elles, le fait de les ajouter à un groupe de sécurité ne change pas la situation. Des passerelles doivent autoriser le trafic qui est défini par les groupes de sécurité sélectionnés.

Si votre compte est activé pour l'adressage privé personnalisé et pour les groupes de sécurité, sachez que les groupes de sécurité relèvent du niveau de compte et non du niveau de réseau. Les groupes de sécurité sont définis par les adresses IP et non par les réseaux privés.

Les groupes de sécurité sont actuellement disponibles dans les centres de données suivants :

| Centres de données      | 
|:------------------|
| AMS01             |
| AMS03             |
| CHE01             |
| DAL01             |
| DAL05             |
| DAL06             |
| DAL09             |
| DAL10             |
| DAL12             |
| DAL13             |
| FRA02             |
| FRA04             |
| FRA05             |
| HKG02             |
| HOU02             |
| LON02             |
| LON04             |
| LON06             |
| MEL01             |
| MEX01             |
| MIL01             |
| MON01             |
| OSL01             |
| PAR01             |
| SAO01             |
| SEA01             |
| SEO01             |
| SJC01             |
| SJC03             |
| SJC04             |
| SNG01             |
| SYD01             |
| SYD04             |
| TOK02             |
| TOR01             |
| WDC01             |
| WDC04             |
| WDC06             |
| WDC07             |
{: caption="Tableau 2. Centre de données prenant en charge les groupes de sécurité" caption-side="top"} 
