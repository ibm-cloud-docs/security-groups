---

copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: create, rules, assign, interface, virtual server

subcollection: security-group
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}


# Création de groupes de sécurité et de règles
{: #creating-security-groups}

Vous pouvez créer un groupe de sécurité et ses règles associées, puis l'affecter aux interfaces de l'une ou de plusieurs instances de serveur virtuel pour activer un pare-feu virtuel.

## Création d'un groupe de sécurité
{: #creating-a-security-group-1}

Pour créer un groupe de sécurité, procédez comme suit :

1. Dans le [portail client ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://cloud.ibm.com/classic), sélectionnez **Sécurité -> Sécurité du réseau -> Groupes de sécurité**.
2. Sur la page Groupes de sécurité, cliquez sur **Créer un groupe**.
3. Entrez un nom et une description pour le groupe de sécurité et cliquez de nouveau sur **Créer un groupe**.

L'option **Créer un groupe avec une règle par défaut pour permettre tout le trafic sortant** est sélectionnée par défaut. Vous pouvez la désactiver pour créer un groupe de sécurité sans règles. Un groupe de sécurité sans règles bloque l'ensemble du trafic (entrant et sortant).
{: note}

## Création des règles du groupe de sécurité
{: #creating-security-group-rules}

Pour créer une règle d'un groupe de sécurité, procédez comme suit :

1. Dans le volet de navigation du [portail client ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://cloud.ibm.com/classic), sélectionnez **Sécurité > Sécurité du réseau > Groupes de sécurité**.
2. Sur la page Groupes de sécurité, cliquez sur le nom d'un groupe de sécurité pour ouvrir la page Détails, puis sélectionnez **Créer une règle**.
3. Sur la page Créer une règle, entrez tous les attributs appropriés (sens, type d'IP, protocole et informations relatives à la source et à la destination, par exemple). Quand vous avez terminé, cliquez sur **OK**.

La sélection facultative des zones Source ou Destination restreignant la nouvelle règle, elle ne s'applique qu'au trafic entrant/sortant de la source/destination spécifiée. Les zones Source ou Destination peuvent spécifier un bloc CIDR (Classless Inter-Domain Routing) ou un groupe de sécurité.
{: note}

Un bloc CIDR facilite le routage d'un bloc d'adresses IP.  Si vous sélectionnez le type CIDR, spécifiez une plage d'adresses IP.

Si vous choisissez le type des groupes de sécurité, sélectionnez une entrée dans la liste des groupes de sécurité existants. De cette manière, toutes les adresses IP d'un périphérique lié au groupe de sécurité sélectionné sont autorisées. Si un serveur virtuel est configuré pour avoir plusieurs adresses IP, seules les adresses principales IPv4 et IPv6 sont utilisées par les règles de ce groupe de sécurité distant.
