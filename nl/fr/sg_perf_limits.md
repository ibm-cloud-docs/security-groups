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

# Limites de performances pour les groupes de sécurité
{: #performance-limitations-for-security-groups}

Il existe certaines limites de performances pour les groupes de sécurité et leurs règles associées.
{: shortdesc}

| Ressource                                                  | Limites                                               |
| --------------------------------------------------------- | --------------------------------------------------- |
| Groupes de sécurité par interface réseau                     | 5                                                   |
| Groupes de sécurité par compte                               | 500                                                 |
| Règles par groupe de sécurité                                  | 50                                                  |
| Règles distantes par groupe de sécurité                           | 5                                                   |
| Interfaces réseau par groupe de sécurité                     | 100                                                  |
{: caption="Tableau 3. Limites de performances pour les ressources spécifiques" caption-side="top"}

Une règle distante est une règle qui définit un groupe de sécurité comme étant la source ou la destination.
{: note}
