---



copyright:
  years: 2017
lastupdated: "2017-04-27"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# Sicherheitsgruppen und Regeln erstellen
{: #creating-security-groups}

Sie können eine Sicherheitsgruppe und ihr zugeordnete Regeln erstellen und sie anschließend den Schnittstellen mindestens einer virtuellen Serverinstanz zuordnen, um eine virtuelle Firewall zu aktivieren.
{:shortdesc}

## Sicherheitsgruppe erstellen

Führen Sie die folgenden Schritte aus, um eine Sicherheitsgruppe zu erstellen:
{:shortdesc}
 
1. Wählen Sie in der Navigation des [Kundenportals ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/) die Optionen für **Sicherheit -> Netzsicherheit -> Sicherheitsgruppen** aus.
2. Klicken Sie auf der Seite 'Sicherheitsgruppen' auf die Option für **Gruppe erstellen**.
3. Geben Sie einen Namen und eine Beschreibung für die Sicherheitsgruppe ein und klicken Sie erneut auf **Gruppe erstellen**.

**Hinweis:** Standardmäßig ist die Option ausgewählt, bei der eine Gruppe mit einer Standardregel erstellt wird, die jeglichen abgehenden Datenverkehr zulässt. Sie können dieses Feld abwählen, damit die Sicherheitsgruppe ohne Regeln erstellt wird. Eine Sicherheitsgruppe ohne Regeln blockiert sämtlichen Datenverkehr (sowohl eingehenden als auch abgehenden).

## Regeln für Sicherheitsgruppen erstellen

Führen Sie die folgenden Schritte aus, um eine Sicherheitsgruppenregel zu erstellen:
{:shortdesc}

1. Wählen Sie in der Navigation des [Kundenportals ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/) die Optionen für **Sicherheit -> Netzsicherheit -> Sicherheitsgruppen** aus.
2. Klicken Sie auf der Seite 'Sicherheitsgruppen' auf den Namen einer Sicherheitsgruppe, um die Seite 'Details' zu öffnen.
3. Geben Sie auf der Detailseite für die Sicherheitsgruppe alle entsprechenden Aktionen ein (wie beispielsweise Richtung, IP-Typ, Protokoll und Informationen zu Quelle/Ziel). Klicken Sie anschließend auf die Option für **Regel erstellen**.

**Hinweis**: In den Feldern für Quelle und Ziel können Sie entweder den Classless Inter-Domain Routing-Block (CIDR) oder die Sicherheitsgruppe angeben. 

Ein CIDR-Block erleichtert die Weiterleitung eines Blocks von IP-Adressen.  Wenn Sie als Typ CIDR auswählen, müssen Sie einen IP-Adressbereich angeben. 

Wenn Sie als Typ Sicherheitsgruppen auswählen, müssen Sie aus einer Liste mit vorhandenen Sicherheitsgruppen auswählen. Diese Auswahl lässt alle IP-Adressen eines Geräts zu, das an die ausgewählte Sicherheitsgruppe angehängt ist. Wenn ein virtueller Server so konfiguriert ist, dass er mehrere IP-Adressen aufweist, werden von diesen fernen Sicherheitsgruppenregeln nur die primären IPv4- und IPv6-Adressen verwendet.
