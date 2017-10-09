---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Vorhandene Netzkonfigurationen und Sicherheitsgruppen

Vorhandene Netzkonfigurationen werden durch Sicherheitsgruppen erweitert. Daher kann eine Sicherheitsgruppe nicht für mehrere
Netze gelten, die untereinander nicht kommunizieren können. 
{:shortdesc}

Auch wenn Sie virtuelle Serverinstanzen, die nicht miteinander kommunizieren können, einer Sicherheitsgruppe hinzufügen, ändert sich dieses
Verhalten nicht. Gateways müssen den Datenverkehr, der von den ausgewählten Sicherheitsgruppen definiert wird, zulassen.

Wenn Ihr Konto sowohl für eine angepasste private Adressierung (CPA - Custom Private Addressing) als auch für Sicherheitsgruppen aktiviert ist, müssen Sie sich darüber im Klaren sein, dass Sicherheitsgruppen bereichsorientiert auf Kontoebene und nicht auf Netzebene wirksam sind. Sicherheitsgruppen werden durch IP-Adressen und nicht durch private Netze definiert.

Sicherheitsgruppen stehen zurzeit in den folgenden Rechenzentren zur Verfügung:

| Rechenzentren      | 
|:------------------|
| CHE01             |
| DAL12             |
| DAL13             |
| HKG02             |
| LON04             |
| MEL01             |
| MIL01             |
| OSL01             |
| SAO01             |
| SJC04             |
| SYD01             |
| SYD04             |
| TOR01             |
| WDC06             |
| WDC07             |
{: caption="Tabelle 2. Rechenzentren, die Sicherheitsgruppen unterstützen" caption-side="top"} 
