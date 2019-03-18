---



copyright:
  years: 2017
lastupdated: "2018-11-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Vorhandene Netzkonfigurationen und Sicherheitsgruppen
{: #existing-network-configurations-and-security-groups}

Vorhandene Netzkonfigurationen werden durch Sicherheitsgruppen erweitert. Daher kann eine Sicherheitsgruppe nicht für mehrere
Netze gelten, die untereinander nicht kommunizieren können. 
{:shortdesc}

Auch wenn Sie virtuelle Serverinstanzen, die nicht miteinander kommunizieren können, einer Sicherheitsgruppe hinzufügen, ändert sich dieses
Verhalten nicht. Gateways müssen den Datenverkehr, der von den ausgewählten Sicherheitsgruppen definiert wird, zulassen.

Wenn Ihr Konto sowohl für eine angepasste private Adressierung (CPA - Custom Private Addressing) als auch für Sicherheitsgruppen aktiviert ist, müssen Sie sich darüber im Klaren sein, dass Sicherheitsgruppen bereichsorientiert auf Kontoebene und nicht auf Netzebene wirksam sind. Sicherheitsgruppen werden durch IP-Adressen und nicht durch private Netze definiert.

Sicherheitsgruppen sind in allen Rechenzentren mit VSI-Bereitstellung verfügbar.
