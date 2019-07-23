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

# Sicherheitsgruppen verwalten
{: #managing-sg}

Sie können Sicherheitsgruppen im Kundenportal der {{site.data.keyword.cloud}}-Infrastruktur auf der Seite 'Sicherheitsgruppen' oder auf der Seite für die Gerätedetails verwalten.
{: shortdesc}

## Sicherheitsgruppen über die Seite 'Sicherheitsgruppen' verwalten
{: #managing-security-groups-from-security-groups-page}

Führen Sie folgende Schritte aus, um Sicherheitsgruppen über die Seite 'Sicherheitsgruppen' zu verwalten:

1. Wählen Sie in der Navigation des [Kundenportals ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://cloud.ibm.com/classic) die Optionen für **Sicherheit -> Netzsicherheit -> Sicherheitsgruppen** aus.
2. Im Abschnitt 'Sicherheitsgruppen' können Sie einige Verwaltungstasks ausführen.
     * Anzeigen einer Liste von Sicherheitsgruppen.
     * Erstellen einer Gruppe.
     * Bearbeiten von Gruppeninformationen.
     * Duplizieren einer Gruppe.
     * Löschen einer Gruppe.

## Sicherheitsgruppenregeln über die Seite 'Sicherheitsgruppen' verwalten
{: #managing-security-group-rules-from-security-groups-page}

Führen Sie folgende Schritte aus, um Sicherheitsgruppenregeln über die Seite 'Sicherheitsgruppen' zu verwalten:

1. Wählen Sie in der Navigation des [Kundenportals ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://cloud.ibm.com/classic) die Optionen für **Sicherheit -> Netzsicherheit -> Sicherheitsgruppen** aus.
2. Klicken Sie auf den Namen einer Sicherheitsgruppe, um die Detailseite zu öffnen.
3. Im Abschnitt für die Details von Sicherheitsgruppen können Sie einige Verwaltungstasks ausführen.
     * Anzeigen einer Liste von Regeln, die für die Sicherheitsgruppe definiert sind.
     * Erstellen neuer Regeln.
     * Bearbeiten einer Regel.
     * Löschen einer Regel.
     * Anzeigen der virtuellen Serverinstanzen und der zugehörigen Schnittstellen, die der Sicherheitsgruppe zugeordnet sind.

Wenn Sie die letzte Regel in einer Sicherheitsgruppe löschen, wird von dieser Sicherheitsgruppe kein eingehender oder abgehender Datenverkehr zugelassen.{: tip}

## Sicherheitsgruppen über die Seite für Gerätedetails verwalten
{: #managing-security-groups-from-device-details-page}

Führen Sie folgende Schritte aus, um Sicherheitsgruppen über die Seite für Gerätedetails zu verwalten:

1. Wählen Sie im [Kundenportal ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://cloud.ibm.com/classic) die Optionen für **Geräte -> Geräteliste** aus.
2. Wählen Sie den Gerätenamen des virtuellen Servers aus, den Sie bestellt haben. Die Seite mit den Gerätedetails wird geöffnet.
3. Überprüfen Sie auf der Seite für die Gerätedetails, dass Sie sich auf der Registerkarte **Konfiguration** befinden.
4. Im Abschnitt 'Sicherheitsgruppen' können Sie einige Verwaltungstasks ausführen.
     * Anzeigen der Sicherheitsgruppen und -regeln.
     * Zuordnen von Sicherheitsgruppen zu einer Netzschnittstelle einer virtuellen Serverinstanz.
     * Entfernen von Sicherheitsgruppen aus der Netzschnittstelle einer virtuellen Serverinstanz.

     Beim erstmaligen Zuordnen einer vorhandenen Sicherheitsgruppe zu einer Netzschnittstelle (öffentlich oder privat) ist für jede der Schnittstellen ein Neustart erforderlich.  Wenn die öffentlichen und privaten Schnittstellen der Sicherheitsgruppe jedoch gleichzeitig zugeordnet wurden, ist nur ein einziger Neustart erforderlich.  Nach einem Neustart werden Änderungen automatisch angewendet.
     {: important}

     Wenn Sie eine neue Sicherheitsgruppe zuordnen, verhindert dies, dass neue Verbindungen gemäß den Definitionen der Sicherheitsgruppenregeln eingerichtet werden. Vorhandene Socketverbindungen werden jedoch nicht beendet.

     Wenn Sie die letzte Sicherheitsgruppe entfernen, die einer virtuellen Serverinstanz zugeordnet ist, wird der Datenverkehr des virtuellen Servers nicht länger durch Sicherheitsgruppen eingeschränkt. Die Firewall einer Sicherheitsgruppe ist dann nicht mehr vorhanden.
     {: tip}

6. Wenn Sie Ihre Änderungen beendet haben, klicken Sie auf **Speichern**.
