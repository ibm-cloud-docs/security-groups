---



copyright:
  years: 2017
lastupdated: "2018-11-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Configuraciones de red y grupos de seguridad existentes

Los grupos de seguridad aumentan la configuración de red existente. Por lo tanto, un grupo de seguridad no puede abarcar redes que no se puedan comunicar entre sí. 
{:shortdesc}

Si las instancias de servidor virtual no se pueden comunicar entre sí, el hecho de añadirlas a un grupo de seguridad no cambiará este comportamiento. Las pasarelas deben permitir el tráfico definido por los grupos de seguridad seleccionados.

Si su cuenta está habilitada para el direccionamiento privado personalizado (CPA) y para grupos de seguridad, tenga en cuenta que los grupos de seguridad abarcan el nivel de cuenta, pero no el de red. Los grupos de seguridad se definen mediante direcciones IP, no mediante redes privadas.

Los grupos de seguridad están disponibles en todos los centros de datos con suministro de VSI.
