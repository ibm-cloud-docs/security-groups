---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"

keywords: add, order, group

subcollection: security-groups


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# Ajout d'un groupe de sécurité prédéfini lors de la commande
{: #adding-a-pre-defined-security-group-during-ordering}

Cette procédure pas à pas vous montre comment ajouter des groupes de sécurité existants ou prédéfinis, dans les instances, durant le processus de commande.

Vous pouvez vous servir des groupes de sécurité pour appliquer un ensemble de règles de filtrage d'adresses IP qui définissent la façon de gérer le trafic entrant et sortant tant au niveau des interfaces publiques qu'au niveau des interfaces privées d'une instance de serveur virtuel.

![Groupe de sécurité personnalisé](./images/goal2.jpg)

## Ce dont vous avez besoin
{: #what-you-ll-need-2}

Pour cet exemple, les objets et éléments suivants seront utilisés :

| Nom de ressource  | Système d'exploitation | Type | Emplacement | IP/Sous-réseau |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| allow_ssh1 | Non applicable  | Groupe de sécurité | Non applicable | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Instance de serveur virtuel | Dallas 10 Pod 01 | 10.0.0.21 |
|jpmongevsi4.testing.com | Ubuntu 16.04 | Instance de serveur virtuel |	Dallas 10 Pod 01	| 10.0.2.219 |

## Commande d'un groupe de sécurité
{: #order-a-security-group}

Pour commander une instance de serveur virtuel et affecter un groupe de sécurité, procédez comme suit :

1. Dans votre navigateur, ouvrez le [portail client ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://cloud.ibm.com/classic) et connectez-vous à votre compte.
2. Recherchez la section **Commander** et cliquez sur **Unités**.
3. Sur la page Unités, cliquez sur l'option **A l'heure** ou **Au mois** correspondant aux offres de serveur virtuel.
4. Sur la page de commande de configuration de votre serveur Cloud, vous devez sélectionner un centre de données qui prend en charge les groupes de sécurité.
5. Renseignez les autres informations requises et cliquez sur l'option d'**ajout à la commande**. La page de réservation s'ouvre.
6. Confirmez les informations suivantes pour l'instance de serveur virtuel :

	* Emplacement
	* Spécifications
	* Options de port réseau.

7. Depuis l'option de configuration des groupes de sécurité, sélectionnez le groupe de sécurité que vous voulez appliquer. Les règles associées à chaque groupe de sécurité peuvent être affichées en cliquant sur le lien **Voir les règles**.

	![Groupe de sécurité personnalisé](./images/sgs.jpg)

	Vous pouvez sélectionner n'importe quel groupe de sécurité prédéfini à appliquer aux interfaces publiques ou privées du serveur virtuel.

8. Spécifiez le nom de l'instance.
9. Cochez, le cas échéant, les cases relatives aux conditions des services Cloud et au contrat de service tiers.
10. Pour terminer, cliquez sur **Soumettre une commande**.
