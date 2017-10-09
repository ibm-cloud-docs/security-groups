---



copyright:
  years: 2017
lastupdated: "2017-08-08"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Instructions relatives aux groupes de sécurité
Tenez compte des instructions suivantes lorsque vous travaillez avec des groupes de sécurité :

## Règles

* Chaque groupe de sécurité spécifie plusieurs ensembles de règles de réseau qui définissent le trafic entrant et sortant d'une instance de serveur virtuel. Vous pouvez spécifier des règles à la fois pour IPv4 et pour IPv6.
* Lorsqu'un nouveau groupe de sécurité est créé à l'aide de l'interface du portail client, le comportement par défaut consiste à créer une seule règle qui autorise l'ensemble du trafic sortant à partir de l'instance de serveur virtuel. Décochez l'option "Créer un groupe avec une règle par défaut pour permettre tout le trafic sortant" pour créer le groupe de sécurité sans règles. Un groupe de sécurité sans règles bloque l'ensemble du trafic (entrant et sortant).
* Pour accepter le trafic entrant et/ou le trafic sortant, vous devez ajouter au moins un groupe de sécurité qui comporte des règles autorisant le trafic. 
* Seules les règles de groupe de sécurité sont permissives. Le trafic est quant à lui bloqué par défaut.
* Les utilisateurs dotés du privilège de gestion des groupes de sécurité peuvent ajouter, éditer ou supprimer des règles dans un groupe de sécurité. 
* Les modifications apportées aux règles de groupe de sécurité sont automatiquement appliquées et peuvent être éditées à tout moment.
* L'ordre des règles au sein du groupe de sécurité n'a pas d'importance. La priorité est toujours accordée à la règle la moins restrictive.
* Les groupes de sécurité ne priment pas sur les pare-feux du système d'exploitation situés sur le serveur virtuel. Si un pare-feu du système d'exploitation est plus restrictif que celui appliqué par les groupes de sécurité, les règles du système d'exploitation sont toujours appliquées.
* Si votre serveur virtuel a besoin d'accéder à des services internes, tels qu'un serveur de mises à jour, un serveur d'accès au réseau ou un contrôle avancé, assurez-vous que les règles de groupes de sécurité tiennent compte du trafic de ces services. Pour plus d'informations, voir [What IP ranges do I allow through the firewall? ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://knowledgelayer.softlayer.com/faqs/6#154) et [Accessing Block Storage on Linux ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://knowledgelayer.softlayer.com/procedure/block-storage-linux).

## Interfaces

* Un groupe de sécurité peut être appliqué à un réseau privé, à un réseau public ou aux deux types d'interface réseau.
* Vous pouvez associer un ou plusieurs groupes de sécurité à la liste des groupes de sécurité attribués à une interface réseau. Les règles de chaque groupe de sécurité s'appliquent aux instances de serveurs virtuels. 
* Lorsque vous affectez un groupe de sécurité existant à une interface réseau (publique ou privée) pour la première fois, vous devez redémarrer chacune des interfaces.  Toutefois, si les interfaces publique et privée ont été affectées simultanément au groupe de sécurité, un seul redémarrage est requis.  Après le redémarrage du système, les modifications sont automatiquement appliquées.

## Accès
 
* Tous les utilisateurs d'un compte peuvent lire, joindre et détacher des groupes de sécurité sur les instances de serveur virtuel auxquelles ils ont accès. Seuls les utilisateurs dotés du privilège de gestion des groupes de sécurité dans les autorisations réseau peuvent créer, mettre à jour et supprimer des groupes de sécurité.
* Vous ne pouvez pas affecter de groupes de sécurité à des serveurs bare metal.

## Suppression

* Vous ne pouvez pas supprimer un groupe de sécurité qui est affecté à une ou plusieurs instances de serveur virtuel en cours d'exécution.
* Vous ne pouvez pas supprimer un groupe de sécurité qui est référencé par un autre groupe de sécurité dans l'une de ses règles. 
