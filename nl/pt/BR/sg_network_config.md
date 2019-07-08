---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: configuration, network, virtual server, instance, security

subcollection: security-group


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# Configurações de rede e grupos de segurança existentes
{: #existing-network-configurations-and-security-groups}

Um grupo de segurança aumenta qualquer configuração de rede existente. Portanto, um grupo de segurança não pode abranger redes que não podem se comunicar
entre si.
{: shortdesc}

Se as instâncias de servidor virtual não podem se comunicar entre si, incluí-las em um grupo de segurança não muda esse
comportamento. Os gateways devem permitir o tráfego definido pelos grupos de segurança selecionados.

Se a sua conta está ativada para o custom private addressing (CPA), bem como grupos de segurança, esteja ciente de que os grupos de segurança têm o escopo definido para o nível de conta, não no nível de rede. Os grupos de segurança são definidos por endereços IP, não redes privadas.

Os grupos de segurança estão disponíveis em todos os data centers com fornecimento de VSI.
