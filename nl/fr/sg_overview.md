---



copyright:
  years: 2017
lastupdated: "2017-08-08"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# A propos des groupes de sécurité

## Qu'est-ce qu'un groupe de sécurité ?
Un *groupe de sécurité* est un ensemble de règles de filtrage d'adresses IP qui détermine la manière de gérer le trafic entrant (ingress) et sortant (egress) tant au niveau des interfaces publiques qu'au niveau des interfaces privées d'une instance de serveur virtuel. Les règles que vous ajoutez à un groupe de sécurité sont dénommées *règles de groupe de sécurité*.
{:shortdesc}

* Vous pouvez affecter des groupes de sécurité aux interfaces réseau publiques et/ou privées d'un seul serveur virtuel ou à plusieurs instances de serveur virtuel.
* Vous pouvez affecter des groupes de sécurité fournis par IBM ou que vous avez créés.
* Lorsqu'un groupe de sécurité est appliqué à un composant réseau d'une instance de serveur virtuel, tout le trafic entrant ou sortant de ce composant réseau est refusé, sauf si une règle de groupe de sécurité l'autorise explicitement.
* Le trafic entrant sur une instance de serveur virtuel est appelé "ingress".
* Le trafic sortant d'une instance de serveur virtuel est appelé "egress".

## Groupes de sécurité fournis par IBM
Vous pouvez affecter n'importe lequel des groupes de sécurité suivants fournis par IBM aux interfaces réseau de vos instances de serveur virtuel :

* *allow_ssh* : ce groupe de sécurité définit les règles d'adresses IP qui autorisent le trafic d'entrée TCP sur le port SSH uniquement (22/TCP).
* *allow_http* : ce groupe de sécurité définit les règles d'adresses IP qui autorisent le trafic d'entrée sur le port HTTP uniquement (80/TCP).
* *allow_https* : ce groupe de sécurité définit les règles d'adresses IP qui autorisent le trafic d'entrée TCP sur le port HTTPS uniquement (443/TCP).
* *allow_outbound* : ce groupe de sécurité définit les règles d'adresses IP qui autorisent l'ensemble du trafic de sortie depuis le serveur.
* *allow_all* : ce groupe de sécurité définit les règles d'adresses IP qui autorisent l'ensemble du trafic d'entrée sur tous les ports.

Dans le diagramme suivant, les instances de serveur virtuel sont associées à un ensemble de groupes de sécurité pour restreindre le trafic réseau.
Les flèches représentent le flux du trafic réseau. Le développeur d'applications a restreint l'accès aux différentes couches de l'infrastructure, comme suit :

* Le développeur d'applications ne peut accéder qu'à la couche Web sur le port TCP 443 (https).
* Seules les instances de la couche Web peuvent accéder aux instances de la couche Application.
* Seules les instances de la couche Application peuvent accéder aux instances de la couche Base de données. 

![Image du groupe de sécurité](images/SecurityGroups.png "Image présentant le flux du trafic réseau avec un ensemble de groupes de sécurité activés") Figure 1. Image du groupe de sécurité


