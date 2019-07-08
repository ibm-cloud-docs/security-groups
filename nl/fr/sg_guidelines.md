---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: security, guidelines, rules

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# Instructions concernant les groupes de sécurité
{: #security-groups-guidelines}

Tenez compte des instructions suivantes lorsque vous travaillez avec des groupes de sécurité :

## Règles
{: #rules-1}

* Chaque groupe de sécurité spécifie plusieurs ensembles de règles de réseau qui définissent le trafic entrant et sortant d'une instance de serveur virtuel. Vous pouvez spécifier des règles à la fois pour IPv4 et pour IPv6.
* Lorsqu'un nouveau groupe de sécurité est créé à l'aide de l'interface du portail client, le comportement par défaut consiste à créer une seule règle qui autorise l'ensemble du trafic sortant à partir de l'instance de serveur virtuel. Décochez l'option "Créer un groupe avec une règle par défaut pour permettre tout le trafic sortant" pour créer le groupe de sécurité sans règles. Un groupe de sécurité sans règles bloque l'ensemble du trafic (entrant et sortant).
* Pour accepter le trafic entrant et/ou le trafic sortant, vous devez ajouter au moins un groupe de sécurité qui comporte des règles autorisant le trafic.
* Seules les règles de groupe de sécurité sont permissives. Le trafic est quant à lui bloqué par défaut.
* Les utilisateurs dotés du privilège de gestion des groupes de sécurité peuvent ajouter, éditer ou supprimer des règles dans un groupe de sécurité.
* Les modifications apportées aux règles de groupe de sécurité sont automatiquement appliquées et peuvent être éditées à tout moment.
* L'ordre des règles au sein du groupe de sécurité n'a pas d'importance. La priorité est toujours accordée à la règle la moins restrictive.
* Des états sont associés aux règles. Les connexions établies avant la modification d'un groupe de sécurité ne seront pas modifiées. Les nouvelles connexions respecteront les règles existant au moment où la connectivité est établie.
* Les groupes de sécurité ne priment pas sur les pare-feux du système d'exploitation situés sur le serveur virtuel. Même s'il existe un pare-feu plus restrictif sur le système d'exploitation que celui appliqué par le groupe de sécurité, les règles du système d'exploitation seront néanmoins appliquées. 
* Si votre serveur virtuel a besoin d'accéder à des services internes, tels qu'un serveur de mises à jour, un serveur d'accès au réseau ou un contrôle avancé, assurez-vous que les règles de groupes de sécurité tiennent compte du trafic de ces services. Pour plus d'informations, voir [Quelles plages d'adresses IP autoriser via le pare-feu](/docs/infrastructure/hardware-firewall-dedicated?topic=hardware-firewall-dedicated-ibm-cloud-ip-ranges).

## Interfaces
{: #interfaces-1}

* Un groupe de sécurité peut être appliqué à un réseau privé, à un réseau public ou aux deux types d'interface réseau.
* Vous pouvez associer un ou plusieurs groupes de sécurité à la liste des groupes de sécurité attribués à une interface réseau. Les règles de chaque groupe de sécurité s'appliquent aux instances de serveurs virtuels.
* Lorsque vous affectez un groupe de sécurité existant à une interface réseau (publique ou privée) pour la première fois, vous devez redémarrer chacune des interfaces.  Toutefois, si les interfaces publique et privée ont été affectées simultanément au groupe de sécurité, un seul redémarrage est requis.  Après le redémarrage du système, les modifications sont automatiquement appliquées.

## Accès
{: #access-1}

* Tous les utilisateurs d'un compte peuvent lire, joindre et détacher des groupes de sécurité sur les instances de serveur virtuel auxquelles ils ont accès. Seuls les utilisateurs dotés du privilège de gestion des groupes de sécurité dans les autorisations réseau peuvent créer, mettre à jour et supprimer des groupes de sécurité.
* Vous ne pouvez pas affecter de groupes de sécurité à des serveurs bare metal.

## Suppression
{: #deletion-1}

* Vous ne pouvez pas supprimer un groupe de sécurité qui est affecté à une ou plusieurs instances de serveur virtuel en cours d'exécution.
* Vous ne pouvez pas supprimer un groupe de sécurité qui est référencé par un autre groupe de sécurité dans l'une de ses règles.
