---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Initiation aux groupes de sécurité
{: #getting-started-with-security-groups}

Vous pouvez vous servir des groupes de sécurité pour appliquer un ensemble de règles de filtrage d'adresses IP qui définissent la façon de gérer le trafic entrant et sortant tant au niveau des interfaces publiques qu'au niveau des interfaces privées d'une instance de serveur virtuel.
{:shortdesc}

Pour commencer, commandez une instance de serveur virtuel et affectez-lui un groupe de sécurité.
 
1. Dans votre navigateur, ouvrez le [Portail client ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com/) et connectez-vous à votre compte.
2. Recherchez la section **Commander** et cliquez sur **Unités**.
3. Sur la page Unités, cliquez sur l'option **A l'heure** ou **Au mois** correspondant aux offres de serveur virtuel.
4. Sur la page de commande de configuration de votre serveur Cloud, vous devez sélectionner un centre de données qui prend en charge les groupes de sécurité.
5. Renseignez les autres informations requises et cliquez sur l'option d'**ajout à la commande**. La page de réservation s'ouvre.
6. Complétez les informations de configuration des groupes de sécurité.
7. Vous pouvez sélectionner n'importe quel groupe de sécurité prédéfini à appliquer aux interfaces publiques ou privées du serveur virtuel.
8. Pour terminer, cliquez sur **Soumettre une commande**.

## Cas d'utilisation et solutions
Les sections ci-après décrivent quelques scénarios de sécurité réseau compliqués auxquels vous pouvez être confronté, dont il est possible d'atténuer la complexité en utilisant les groupes de sécurité.

### Sécurité dès la mise à disposition
**Scénario de sécurité :** les clients veulent sécuriser leur serveur virtuel dès qu'il est mis à disposition. Ils veulent disposer d'un contrôle complet sur le trafic passant sur le serveur, depuis le point où ce dernier a été mis à disposition.

**Solution :** utilisez les groupes de sécurité au moment de la commande du serveur virtuel. De cette façon, votre serveur est protégé dès le moment de sa mise à disposition.

### Pare-feu de niveau instance d'un bon rapport qualité/prix
**Scénario de sécurité :** les clients veulent disposer d'un contrôle très précis sur le trafic au niveau d'une instance (sans parler du niveau réseau), mais d'un autre côté, les coûts générés par un pare-feu matériel partagé (autre offre de pare-feu à service partagé proposé par IBM©) peuvent augmenter rapidement si les clients ont besoin de protéger des serveurs multiples dans différents centres de données.

**Solution :** l'utilisation de la fonction Groupes de sécurité ne génère pas de coût supplémentaire. Servez-vous des groupes de sécurité pour tous les serveurs virtuels nécessitant une protection dans l'un de nos centres de données internationaux.

### Pare-feu à évolution globale et gestion aisée
**Scénario de sécurité :** les clients veulent éviter d'avoir à configurer des règles de pare-feu sur chaque serveur séparément. Ils préfèrent disposer d'une solution de pare-feu facilement gérable qui s'applique sur divers serveurs dans différents centres de données internationaux.

**Solution :** définissez `N` groupes de sécurité pour `N` types de serveurs différents dans votre charge de travail de cloud. Gérez toutes les règles pour un groupe de sécurité dans un emplacement unique. Gérez les associations de groupe de sécurité de façon appropriée avec les serveurs virtuels.
