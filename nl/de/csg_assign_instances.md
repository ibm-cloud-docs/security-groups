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

# Instanzen zu der Sicherheitsgruppe zuordnen
Sie haben zwei Möglichkeiten, Sicherheitsgruppenobjekte zu Instanzen zuzuordnen:

## Über das Sicherheitsmenü

1. Wählen Sie auf der Registerkarte **Sicherheit** im [Kundenportal ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} unter **Netzsicherheit** den Eintrag **Sicherheitsgruppen** aus.
2. Klicken Sie auf das Symbol ![Symbol 'Mehr'](./images/more_icon.jpg) des Sicherheitsgruppenobjekts, dem Sie Instanzen zuordnen möchten, und wählen Sie dann **Instanzen verwalten** aus.
3. Wählen Sie die Instanz und die Schnittstelle aus, die auf die Sicherheitsgruppe angewendet werden sollen.

	![Sicherheitsmenü-Instanz](./images/security_assign.jpg)

	In der Abbildung wird die Sicherheitsgruppe 'allow_icmp' (erstellt im [ersten Schritt](csg_create.html)) auf die private Schnittstelle (`10.0.2.219`) 'jpmongevsi4' angewendet.

	Beachten Sie, dass sich die Anzahl **Angehängte Instanzen** von `0` in `1` geändert hat.

4. Klicken Sie auf **Speichern**, um die Änderungen anzuwenden.

5. Starten Sie Ihre Instanz neu.

	**HINWEIS:** Dieser Schritt muss für Instanzen, die nicht mit einer Sicherheitsgruppe erstellt wurden, nur einmal pro Netzschnittstelle ausgeführt werden.

## Über das Gerätemenü

1. Wählen Sie auf der Registerkarte **Geräte** im [Kundenportal ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} den Eintrag **Geräteliste** aus.
2. Klicken Sie auf den Namen der Instanz, in der Sie das Sicherheitsgruppenobjekt anwenden möchten.
3. Wählen Sie **Ändern** aus und markieren Sie das Sicherheitsgruppenobjekt, das Sie der Instanz zuordnen möchten.

	![Gerätemenü-Instanz](./images/device_assign.jpg)

	In dieser Abbildung wird das Sicherheitsgruppenobjekt 'allow_icmp' der privaten Schnittstelle der Instanz 'jpmongevsi4' zugeordnet.
4. Klicken Sie auf **Speichern**, um die Änderungen anzuwenden.

5. Starten Sie die Instanz neu.

	**HINWEIS:** Dieser Schritt muss für Instanzen, die nicht mit einer Sicherheitsgruppe erstellt wurden, nur einmal pro Netzschnittstelle ausgeführt werden.

## Nächster Schritt ...
[Sicherheitsgruppe bearbeiten](csg_edit.html), um die zugehörigen Parameter zu ändern.  