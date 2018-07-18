---



copyright:
  years: 2017, 2018
lastupdated: "2018-04-04"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Einführung in Sicherheitsgruppen

Sie können Sicherheitsgruppen verwenden, um eine Gruppe von IP-Filterregeln einzurichten, die definieren, wie eingehender und abgehender Datenverkehr an bzw. von sowohl öffentlichen als auch privaten Schnittstellen einer virtuellen Serverinstanz gehandhabt wird.
{:shortdesc}

Bestellen Sie zunächst eine virtuelle Serverinstanz (VSI) und ordnen Sie eine Sicherheitsgruppe zu. 
 
1. Öffnen Sie in Ihrem Browser das [Kundenportal ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/) und melden Sie sich mit Ihrem Konto an. 
2. Suchen Sie nach dem Abschnitt **Bestellung** und klicken Sie auf **Geräte**. 
3. Klicken Sie auf der Seite 'Geräte' für eines der Angebote für einen virtuellen Server auf die Option **Stündlich** oder **Monatlich**. 
4. Auf der Bestellseite zum Konfigurieren Ihres Cloud-Servers**** müssen Sie ein Rechenzentrum auswählen, das Sicherheitsgruppen unterstützt.
5. Füllen Sie alle weiteren erforderlichen Informationen aus und klicken Sie auf die Option für **Zur Bestellung hinzufügen**. Die Kassenseite wird geöffnet. 
6. Füllen Sie die Informationen für die Konfiguration**** von Sicherheitsgruppen aus.
7. Sie können eine beliebige der vordefinierten Sicherheitsgruppen auswählen, die dann auf die privaten oder öffentlichen Schnittstellen auf dem virtuellen Server angewendet wird. 
8. Klicken Sie zuletzt auf die Option für **Bestellung abschicken**. 

## Anwendungsfälle und Lösungen
In den folgenden Abschnitten werden einige schwierige Netzsicherheitsszenarios beschrieben, die mithilfe von Sicherheitsgruppen vereinfacht werden können. 

### Sicherheit von Beginn an
**Sicherheitsszenario:** Kunden möchten ihre virtuellen Server ab dem Zeitpunkt ihrer Bereitstellung sichern. Sie möchten vollständige Kontrolle über den Datenverkehr, der den Server passiert, ab dem Zeitpunkt seiner Bereitstellung. 

**Lösung:** Verwenden Sie Sicherheitsgruppen, wenn Sie den virtuellen Server bestellen. Auf diese Weise ist Ihr Server ab dem Zeitpunkt seiner Bereitstellung geschützt. 

### Kosteneffiziente Firewall auf Instanzebene
**Sicherheitsszenario:** Kunden möchten differenzierte Kontrolle über den Datenverkehr auf Instanzebene (abgesehen von dem Einsatz von Firewalls auf Netzebene), aber gleichzeitig können sich die Kosten einer gemeinsam genutzten Hardware-Firewall (IBMs anderes Multi-Tenant-Firewall-Angebot auf Instanzebene) schnell summieren, wenn der Kunde mehrere Server in verschiedenen Rechenzentren schützen muss. 

**Lösung:** Die Verwendung des Features 'Sicherheitsgruppen' wird nicht extra berechnet. Verwenden Sie Sicherheitsgruppen für alle virtuellen Server, die geschützt werden müssen, in allen globalen Rechenzentren. 

### Global skalierbare und einfach zu verwaltende Firewall
**Sicherheitsszenario:** Kunden möchten vermeiden, Firewallregeln auf jedem Server separat zu konfigurieren. Stattdessen wünschen sie sich eine einfach zu verwaltende Firewalllösung für Server in verschiedenen globalen Rechenzentren. 

**Lösung:** Definieren Sie `N` Sicherheitsgruppen für `N` verschiedene Arten von Servern in Ihrer Cloud-Workload. Verwalten Sie alle Regeln für eine Sicherheitsgruppe an einem zentralen Ort. Verwalten Sie die Sicherheitsgruppenzuordnungen entsprechend mit den virtuellen Servern. 
