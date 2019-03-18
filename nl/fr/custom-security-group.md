---



copyright:
  years: 2017
lastupdated: "2018-11-10"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Création et gestion d'un groupe de sécurité personnalisé
{: #creating-and-managing-a-custom-security-group}

Dans ce tutoriel, vous allez apprendre à créer et à affecter des instances, et à éditer un groupe de sécurité personnalisé.

![Groupe de sécurité personnalisé](./images/goal.jpg)

## Ce dont vous avez besoin
Pour cet exemple, les objets et éléments suivants seront utilisés :

| Nom de ressource  | Système d'exploitation | Type | Emplacement | IP/Sous-réseau |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| Non applicable | 10.0.0.0/16 |
| allow_icmp | Non applicable  | Groupe de sécurité | Non applicable | 0.0.0.0/0 |
| allow_ssh | Non applicable | Groupe de sécurité | Non applicable | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Instance de serveur virtuel | Dallas 10 Pod 01 | 10.0.0.21 |
|jpmongevsi4.testing.com | Ubuntu 16.04 | Instance de serveur virtuel |	Dallas 10 Pod 01	| 10.0.2.219 |


Notez que ce tutoriel utilise un compte/réseau privé CPA (Custom Private Addressing). Toutefois, pour des raisons pratiques, les groupes de sécurité se comportent de la même façon dans les comptes CPA que dans les comptes ordinaires. Les sous-réseaux 10.0.0.0/24 et 10.0.2.0/24 appartiennent au même réseau privé CPA, ce qui équivaut à avoir un compte ordinaire avec deux instance de serveur virtuel ou plus connectées au même sous réseau/VLAN.


## Ce que vous allez faire

Dans ce tutoriel. vous allez apprendre à...

Tâche  | Description
------------- | -------------
[Créer un groupe de sécurité](/docs/infrastructure/security-groups?topic=security-groups-creating-a-security-group) | Créez et configurez un groupe de sécurité personnalisé, plutôt que d'utiliser un groupe prédéfini proposé par la plateforme IBM© Cloud. 
[Créer une règle](/docs/infrastructure/security-groups?topic=security-groups-creating-a-new-rule) | Créez une règle pour autoriser les demandes entrantes (SSH et ICMP) et les flux de trafic (en sortie) associés
[Affecter des instances au groupe de sécurité](/docs/infrastructure/security-groups?topic=security-groups-assigning-instances-to-the-security-group) | Affectez des objets Groupe de sécurité aux instances en utilisant le menu Sécurité ou le menu Unité.
[Editer un groupe de sécurité et ses règles](/docs/infrastructure/security-groups?topic=security-groups-editing-a-security-group) | Modifiez les paramètres de l'objet Sécurité et de ses règles.
