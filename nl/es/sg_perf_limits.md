---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: performance, limits, limitations, rules

subcollection: security-group


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# Limitaciones de rendimiento para los grupos de seguridad
{: #performance-limitations-for-security-groups}

Hay algunas limitaciones de rendimiento para los grupos de seguridad y las reglas asociadas correspondientes.
{: shortdesc}

| Recurso                                                  | Límite                                               |
| --------------------------------------------------------- | --------------------------------------------------- |
| Grupos de seguridad por interfaz de red                     | 5                                                   |
| Grupos de seguridad por cuenta                               | 500                                                 |
| Reglas por grupo de seguridad                                  | 50                                                  |
| Reglas remotas por grupo de seguridad                           | 5                                                   |
| Interfaces de red por grupo de seguridad                     | 100                                                  |
{: caption="Tabla 3. Limitaciones de rendimiento para recursos específicos" caption-side="top"}

Las reglas remotas son aquellas que especifican un grupo de seguridad como origen o destino.
{: note}
