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
| CHE01             |
| DAL12             |
| DAL13             |
| HKG02             |
| LON04             |
| MEL01             |
| MIL01             |
| OSL01             |
| SAO01             |
| SJC04             |
| SYD01             |
| SYD04             |
| TOR01             |
| WDC06             |
| WDC07             |
{: caption="Tabla 2. Centros de datos que soportan grupos de seguridad" caption-side="top"} 
