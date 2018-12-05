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

# Schritt für Schritt: Hinzufügen einer vordefinierten Sicherheitsgruppe während der Bestellung
Dieses schrittweises Vorgehen zeigt Ihnen, wie Sie vorhandene oder vordefinierte Sicherheitsgruppen während des Bestellablaufs zu Instanzen hinzufügen.

Sie können Sicherheitsgruppen verwenden, um eine Gruppe von IP-Filterregeln einzurichten, die definieren, wie eingehender und abgehender Datenverkehr an bzw. von sowohl öffentlichen als auch privaten Schnittstellen einer virtuellen Serverinstanz gehandhabt wird.

![Angepasste Sicherheitsgruppe](./images/goal2.jpg)

## Voraussetzungen
In diesem Beispiel werden die folgenden Objekte und Elemente verwendet:

| Ressourcenname  | Betriebssystem | Typ | Ort/Rechenzentrum | IP/Teilnetz |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| allow_ssh1 | Nicht zutreffend  | Sicherheitsgruppe | Nicht zutreffend/Kein | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Virtuelle Serverinstanz | Dallas 10 Pod 01 | 10.0.0.21 |	
|jpmongevsi4.testing.com | Ubuntu 16.04 | Virtuelle Serverinstanz |	Dallas 10 Pod 01	| 10.0.2.219 |

## Bestellen einer Sicherheitsgruppe
Führen Sie die folgenden Schritte aus, um eine virtuelle Serverinstanz (VSI) zu bestellen und eine Sicherheitsgruppe zuzuordnen.

1. Öffnen Sie in Ihrem Browser das [Kundenportal ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/) und melden Sie sich mit Ihrem Konto an.
2. Suchen Sie nach dem Abschnitt **Bestellung** und klicken Sie auf **Geräte**.
3. Klicken Sie auf der Seite 'Geräte' für eines der Angebote für einen virtuellen Server auf die Option **Stündlich** oder **Monatlich**.
4. Auf der Bestellseite zum Konfigurieren Ihres Cloud-Servers müssen Sie ein Rechenzentrum auswählen, das Sicherheitsgruppen unterstützt.
5. Füllen Sie alle weiteren erforderlichen Informationen aus und klicken Sie auf die Option für **Zur Bestellung hinzufügen**. Die Kassenseite wird geöffnet.
6. Bestätigen Sie die folgenden Informationen für die VSI: 

	* Ort
	* Spezifikationen
	* Netzportoptionen 

7. Wählen Sie in **Sicherheitsgruppen konfigurieren** die anzuwendende Sicherheitsgruppe aus. Die jeder Sicherheitsgruppe zugeordneten Regeln können angezeigt werden, indem Sie auf den Link **Regeln anzeigen** klicken. 

	![Angepasste Sicherheitsgruppe](./images/sgs.jpg)

	Sie können eine beliebige der vordefinierten Sicherheitsgruppen auswählen, die dann auf die privaten oder öffentlichen Schnittstellen auf dem virtuellen Server angewendet wird.
	
8. Geben Sie den Instanznamen an.
9. Markieren Sie ggf. die Kontrollkästchen für die Cloud-Service-Bedingungen und die Drittanbieter-Servicevereinbarung.
10. Klicken Sie zuletzt auf die Option für **Bestellung abschicken**.
