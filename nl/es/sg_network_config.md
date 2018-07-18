---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Configuraciones de red y grupos de seguridad existentes

Los grupos de seguridad aumentan la configuración de red existente. Por lo tanto, un grupo de seguridad no puede abarcar redes que no se puedan comunicar entre sí. 
{:shortdesc}

Si las instancias de servidor virtual no se pueden comunicar entre sí, el hecho de añadirlas a un grupo de seguridad no cambiará este comportamiento. Las pasarelas deben permitir el tráfico definido por los grupos de seguridad seleccionados.

Si su cuenta está habilitada para el direccionamiento privado personalizado (CPA) y para grupos de seguridad, tenga en cuenta que los grupos de seguridad abarcan el nivel de cuenta, pero no el de red. Los grupos de seguridad se definen mediante direcciones IP, no mediante redes privadas.

Los grupos de seguridad actualmente están disponibles en los siguientes centros de datos:

| Centros de datos      | 
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
{: caption="Tabla 2. Centros de datos que soportan grupos de seguridad" caption-side="top"} 
