---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: create, configure, configuration, custom

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:note: .note}
{:important: .important}
{:tip: .tip}
{:table: .aria-labeledby="caption"}

# Création d'un groupe de sécurité
{: #creating-a-security-group}

Créez et configurez un groupe de sécurité personnalisé :

1. Dans votre navigateur, ouvrez le [portail client ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://cloud.ibm.com/classic){: new_window} et connectez-vous à votre compte.
2.	Sélectionnez l'onglet **Sécurité**.
3. Depuis **Sécurité du réseau**, sélectionnez **Groupes de sécurité**.
4.	Cliquez sur **Créer un groupe +**.
5.	Entrez un nom pour le groupe de sécurité et, si vous le souhaitez, une description.
6. Cliquez sur **Créer un groupe**.

![Création d'un groupe de sécurité](./images/create_sg.jpg)

Notez que la case à cocher **Créer un groupe avec une règle par défaut pour permettre tout le trafic sortant** est désélectionnée, ce qui signifie qu'aucune règle sortante ne sera créée pour cet objet Groupe de sécurité. Par conséquent, à moins que d'autres règles sortantes ou objets Groupe de sécurité ne soient créés, seules les demandes entrantes (comme SSH et ICMP) et les réponses et flux de trafic (en sortie) associés seront autorisés.

## Etape suivante...
{: #next-step-2}

[Créez une règle](/docs/infrastructure/security-groups?topic=security-groups-creating-a-new-rule) pour autoriser les demandes entrantes (SSH et ICMP) et les flux de trafic (en sortie) associés.  
