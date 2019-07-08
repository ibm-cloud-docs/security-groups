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

# Leistungseinschränkungen für Sicherheitsgruppen
{: #performance-limitations-for-security-groups}

Für Sicherheitsgruppen und die ihnen zugeordneten Regeln gelten einige Leistungseinschränkungen.
{: shortdesc}

| Ressource                                                  | Beschränkung                                               |
| --------------------------------------------------------- | --------------------------------------------------- |
| Sicherheitsgruppen pro Netzschnittstelle                     | 5                                                   |
| Sicherheitsgruppen pro Konto                               | 500                                                 |
| Regeln pro Sicherheitsgruppe                                  | 50                                                  |
| Ferne Regeln pro Sicherheitsgruppe                           | 5                                                   |
| Netzschnittstellen pro Sicherheitsgruppe                     | 100                                                  |
{: caption="Tabelle 3. Leistungseinschränkungen für bestimmte Ressourcen" caption-side="top"}

Eine ferne Regel ist eine Regel, die eine Sicherheitsgruppe als Quelle oder Ziel angibt.{: note}
