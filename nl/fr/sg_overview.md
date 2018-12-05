---



copyright:
  years: 2017
lastupdated: "2018-11-10"

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

Les groupes de sécurité sont implémentés sur l'hyperviseur hébergeant le serveur virtuel.

## Groupes de sécurité fournis par IBM
Vous pouvez affecter l'un des groupes de sécurité suivants, fournis par IBM, dans les interfaces réseau de vos instances de serveur virtuel :

* *allow_ssh* : ce groupe de sécurité définit les règles d'adresses IP qui autorisent le trafic d'entrée TCP sur le port SSH uniquement (22/TCP).
* *allow_http* : ce groupe de sécurité définit les règles d'adresses IP qui autorisent le trafic d'entrée sur le port HTTP uniquement (80/TCP).
* *allow_https* : ce groupe de sécurité définit les règles d'adresses IP qui autorisent le trafic d'entrée TCP sur le port HTTPS uniquement (443/TCP).
* *allow_outbound* : ce groupe de sécurité définit les règles d'adresses IP qui autorisent l'ensemble du trafic de sortie depuis le serveur.
* *allow_all* : ce groupe de sécurité définit les règles d'adresses IP qui autorisent l'ensemble du trafic d'entrée sur tous les ports.

## Groupes de sécurité et journaux d'audit
Toutes les interactions de groupe de sécurité sont consignées dans un [journal d'audit](/docs/customer-portal/cpmonenv.html#cp_viewacctauditlog) de compte. Les entrées de journal d'audit effectuent le suivi des changements apportés à des groupes de sécurité spécifiques et gardent trace du nom de l'utilisateur qui a demandé la modification. Des entrées sont effectuées dans les journaux pour les interactions suivantes :
* Un groupe de sécurité est ajouté dans une interface réseau de serveur virtuel (ou retiré de cette dernière)
* Les règles d'un groupe de sécurité sont modifiées (ajout, édition ou retrait d'une règle).

Pour chacune de ces interactions, un journal est écrit pour chaque objet affecté. Toute modification d'un groupe de sécurité entraîne l'inscription dans un journal. Des journaux supplémentaires sont écrits pour chaque interface réseau de serveur virtuel attachée au groupe de sécurité. Le filtrage des journaux d'audit sur un groupe de sécurité spécifique montre tous les changements apportés à ce groupe de sécurité pour le groupe. De la même façon, le filtrage des journaux sur un serveur virtuel spécifique affiche toutes les modifications effectuées dans le(s) groupe(s) de sécurité pour le serveur virtuel.

Puisque les modifications apportées aux groupes de sécurité peuvent conduire à une mise à jour en arrière-plan d'un certain nombre de serveurs virtuels, les journaux d'audit permettent de déterminer précisément quand un changement a pris effet.  Les API de groupe de sécurité qui génèrent des journaux d'audit retournent un identificateur de demande. Cet identificateur peut servir à établir une corrélation entre les appels API et les journaux d'audit résultants.

## Exemple
Dans le diagramme suivant, les instances de serveur virtuel sont associées à un ensemble de groupes de sécurité pour restreindre le trafic réseau. Les flèches représentent le flux du trafic réseau. Le développeur d'applications a restreint l'accès aux différentes couches de l'infrastructure, comme suit :

* Le développeur d'applications ne peut accéder qu'à la couche Web sur le port TCP 443 (https).
* Seules les instances de la couche Web peuvent accéder aux instances de la couche Application.
* Seules les instances de la couche Application peuvent accéder aux instances de la couche Base de données. 

![Image du groupe de sécurité](images/SecurityGroups.png "Image présentant le flux du trafic réseau avec un ensemble de groupes de sécurité activés") Figure 1. Image du groupe de sécurité


