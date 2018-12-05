---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Affectation d'instances au groupe de sécurité
Vous pouvez affecter des objets de groupe de sécurité à des instances en utilisant l'une des méthodes suivantes :

## Utilisation du menu Sécurité

1. Depuis l'onglet **Sécurité** du [portail client ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com/){: new_window}, sous **Sécurité du réseau**, sélectionnez **Groupes de sécurité**.
2. Cliquez sur l'![icône Plus](./images/more_icon.jpg) de l'objet Groupe de sécurité auquel vous voulez affecter des instances puis sélectionnez **Gérer des instances**.
3. Sélectionnez l'instance et l'interface à appliquer au groupe de sécurité.

	![Instances affectées](./images/security_assign.jpg)

	Dans cet écran, le groupe de sécurité "allow_icmp" (créé à la [première étape](csg_create.html)) est appliqué à l'interface privée (`10.0.2.219`) de "jpmongevsi4".

	Notez que le compte **Instances jointes** est passé de `0` à `1`.

4. Cliquez sur **Enregistrer** pour appliquer les changements.

5. Redémarrez votre instance.

	**Remarque :** il s'agit d'une étape unique par interface réseau pour les instances qui n'ont pas été créées avec un groupe de sécurité.

## Utilisation du menu Unités

1. Depuis l'onglet **Unités** du [portail client![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://control.softlayer.com/){: new_window}, sélectionnez **Liste des unités**.
2. Cliquez sur le nom de l'instance dans laquelle vous voulez appliquer l'objet Groupe de sécurité.
3. Sélectionnez **Modifier** et marquez l'objet Groupe de sécurité que vous voulez associer à l'instance.

	![Interface réseau privé](./images/device_assign.jpg)

	Cet écran montre l'objet Groupe de sécurité "allow_icmp" qui est affecté à l'interface privée de l'instance jpmongevsi4.
4. Cliquez sur **Enregistrer** pour appliquer les changements.

5. Redémarrez l'instance.

	**Remarque :** il s'agit d'une étape unique par interface réseau pour les instances qui n'ont pas été créées avec un groupe de sécurité.

## Etape suivante...
[Editez le groupe de sécurité](csg_edit.html) pour modifier ses paramètres  
