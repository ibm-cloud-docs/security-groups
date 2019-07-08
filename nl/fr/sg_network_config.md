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

# Configurations réseau existantes et groupes de sécurité
{: #existing-network-configurations-and-security-groups}

Un groupe de sécurité permet d'étendre une configuration réseau existante. Par conséquent, un groupe de sécurité ne peut pas être étendu sur des réseaux incapables de pas communiquer entre eux.
{: shortdesc}

Si des instances de serveur virtuel ne parviennent pas à communiquer entre elles, le fait de les ajouter à un groupe de sécurité ne change pas la situation. Des passerelles doivent autoriser le trafic qui est défini par les groupes de sécurité sélectionnés.

Si votre compte est activé pour l'adressage privé personnalisé et pour les groupes de sécurité, sachez que les groupes de sécurité relèvent du niveau de compte et non du niveau de réseau. Les groupes de sécurité sont définis par les adresses IP et non par les réseaux privés.

Des groupes de sécurité sont disponibles dans tous les centres de données avec mise à disposition d'instances de serveurs virtuels.
