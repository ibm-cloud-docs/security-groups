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

# Limitações de desempenho para grupos de segurança
{: #performance-limitations-for-security-groups}

Existem algumas limitações de desempenho para grupos de segurança e suas regras associadas.
{: shortdesc}

| Resource                                                  | Limite                                               |
| --------------------------------------------------------- | --------------------------------------------------- |
| Grupos de segurança por interface de rede                     | 5                                                   |
| Grupos de segurança por conta                               | 500                                                 |
| Regras para grupo de segurança                                  | 50                                                  |
| Regras remotas por grupo de segurança                           | 5                                                   |
| Interfaces de rede por grupo de segurança                     | 100                                                  |
{: caption="Tabela 3. Limitações de desempenho para recursos específicos" caption-side="top"}

Uma regra remota é aquela que especifica um grupo de segurança como a origem ou o destino.
{: note}
