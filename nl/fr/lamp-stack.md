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

# Application Web sur pile LAMP
Autorisez les demandes entrantes (SSH et ICMP) et les flux de trafic (en sortie) associés en procédant comme suit :

1. Sélectionnez l'onglet **Règles** dans le [portail client![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://cloud.ibm.com/classic){: new_window}.
2.	Cliquez sur **Créer une règle**.
3.	Spécifiez les éléments suivants : Sens (de la règle), Type d'IP, Protocole, Plage de ports, Type, Code et Source, si applicable (selon la sélection effectuée dans Protocole). 

	A moins que vous n'utilisiez un autre groupe de sécurité en tant que source, laissez **Type de source** sur "Bloc CIDR".
	
	![Création d'une règle](rule_sg.jpg)
	
	Cet écran montre **Tout l'ICMP** sélectionné comme protocole, ce qui signifie que tous les codes et types ICMP sont autorisés. De plus, la zone Source reste vide, utilisant la valeur par défaut `0.0.0.0/0` -- équivalent à tout sous-réseau ou adresse IP.

4.	Cliquez sur **OK** pour terminer la procédure.
