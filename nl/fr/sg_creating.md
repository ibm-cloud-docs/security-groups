---



copyright:
  years: 2017
lastupdated: "2017-04-27"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# Création de groupes de sécurité et de règles
{: #creating-security-groups}

Vous pouvez créer un groupe de sécurité et ses règles associées, puis l'affecter aux interfaces de l'une ou de plusieurs instances de serveur virtuel pour activer un pare-feu virtuel.
{:shortdesc}

## Création d'un groupe de sécurité

Pour créer un groupe de sécurité, procédez comme suit :
{:shortdesc}
 
1. Dans le [Portail client ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/), sélectionnez **Sécurité -> Sécurité du réseau -> Groupes de sécurité**.
2. Sur la page Groupes de sécurité, cliquez sur **Créer un groupe**.
3. Entrez un nom et une description pour le groupe de sécurité et cliquez de nouveau sur **Créer un groupe**.

**Remarque :** l'option "Créer un groupe avec une règle par défaut pour permettre tout le trafic sortant" est sélectionnée par défaut. Vous pouvez la désactiver pour créer un groupe de sécurité sans règles. Un groupe de sécurité sans règles bloque l'ensemble du trafic (entrant et sortant).

## Création des règles du groupe de sécurité

Pour créer une règle d'un groupe de sécurité, procédez comme suit :
{:shortdesc}

1. Dans le [Portail client ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/), sélectionnez **Sécurité -> Sécurité du réseau -> Groupes de sécurité**.
2. Sur la page Groupes de sécurité, cliquez sur le nom d'un groupe de sécurité pour ouvrir la page Détails.
3. Dans la page qui s'ouvre, entrez toutes les actions appropriées (direction, type IP, protocole et informations relatives à la source/destination). Une fois terminé, cliquez sur **Créer une règle**.

**Remarque** : dans les zones source et destination, indiquez un groupe de sécurité ou bloc Classless Inter-Domain Routing (CIDR). 

Un bloc CIDR facilite le routage d'un bloc d'adresses IP.  Si vous sélectionnez le type CIDR, spécifiez une plage d'adresses IP. 

Si vous choisissez le type des groupes de sécurité, sélectionnez une entrée dans la liste des groupes de sécurité existants. De cette manière, toutes les adresses IP d'un périphérique lié au groupe de sécurité sélectionné sont autorisées. Si un serveur virtuel est configuré pour avoir plusieurs adresses IP, seules les adresses principales IPv4 et IPv6 sont utilisées par les règles de ce groupe de sécurité distant.
