---



copyright:
  years: 2017, 2019
lastupdated: "2019-06-11"

keywords: manage, details, edit, configure

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# Gestion des groupes de sécurité
{: #managing-sg}

Vous pouvez gérer les groupes de sécurité sur la page Groupes de sécurité du portail client de l'infrastructure {{site.data.keyword.cloud}}.
{: shortdesc}

## Gestion des groupes de sécurité à partir de la page Groupes de sécurité
{: #managing-security-groups-from-security-groups-page}

Pour gérer les groupes de sécurité à partir de la page Groupes de sécurité, procédez comme suit :

1. Depuis le [portail client ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://cloud.ibm.com/classic), sélectionnez **Sécurité -> Sécurité du réseau -> Groupes de sécurité**.
2. Dans la section Groupe de sécurité, vous pouvez effectuer plusieurs tâches de gestion.
     * Afficher la liste des groupes de sécurité.
     * Créer un groupe.
     * Editer les informations sur le groupe.
     * Dupliquer un groupe.
     * Supprimer un groupe.

## Gestion des règles de groupe de sécurité à partir de la page Groupes de sécurité
{: #managing-security-group-rules-from-security-groups-page}

Pour gérer les règles de groupe de sécurité à partir de la page Groupes de sécurité, procédez comme suit :

1. Depuis le [portail client ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://cloud.ibm.com/classic), sélectionnez **Sécurité -> Sécurité du réseau -> Groupes de sécurité**.
2. Cliquez sur le nom d'un groupe de sécurité pour ouvrir la page Détails.
3. Dans la page qui s'ouvre, vous pouvez effectuer plusieurs tâches de gestion.
     * Afficher la liste des règles qui sont définies pour le groupe de sécurité.
     * Créer des règles.
     * Editer une règle.
     * Supprimer une règle.
     * Afficher les instances de serveur virtuel et les interfaces associées qui sont affectées au groupe de sécurité.

Si vous supprimez la dernière règle d'un groupe de sécurité, aucun trafic entrant ni sortant n'est autorisé par ce groupe de sécurité.
{: tip}

## Gestion des groupes de sécurité à partir de la page Détails
{: #managing-security-groups-from-device-details-page}

Pour gérer les groupes de sécurité à partir de la page Détails de l'unité, procédez comme suit :

1. Depuis le [portail client ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://cloud.ibm.com/classic), sélectionnez **Unités -> Liste des unités**.
2. Sélectionnez le nom d'unité du serveur virtuel que vous avez commandé. La page Détails de l'unité s'ouvre.
3. Dans la page Détails de l'unité, vérifiez que vous êtes dans l'onglet **Configuration**.
4. Dans la section Groupe de sécurité, vous pouvez effectuer plusieurs tâches de gestion.
     * Afficher les groupes de sécurité et les règles.
     * Affecter les groupes de sécurité à une interface réseau d'une instance de serveur virtuel.
     * Supprimer des groupes de sécurité d'une interface réseau d'une instance de serveur virtuel.

     Lorsque vous affectez un groupe de sécurité existant à une interface réseau (publique ou privée) pour la première fois, vous devez redémarrer chacune des interfaces.  Toutefois, si les interfaces publique et privée ont été affectées simultanément au groupe de sécurité, un seul redémarrage est requis.  Après le redémarrage du système, les modifications sont automatiquement appliquées.
     {: important}

     Lorsque vous affectez un nouveau groupe de sécurité, celui-ci bloque l'établissement de nouvelles connexions en fonction des définitions de règles du groupe de sécurité. Toutefois, certaines connexions socket ne sont pas terminées.

     Si vous supprimez le dernier groupe de sécurité affecté à une instance de serveur virtuel, le trafic de ce serveur n'est plus limité par les groupes de sécurité. Il n'existe plus aucun pare-feu.
     {: tip}

6. Une fois les modifications terminées, cliquez sur **Sauvegarder**.
