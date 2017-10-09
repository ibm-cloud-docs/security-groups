---



copyright:
  years: 2017
lastupdated: "2017-08-08"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Informationen zu Sicherheitsgruppen

## Definition einer Sicherheitsgruppe
Eine *Sicherheitsgruppe* ist eine Gruppe von IP-Filterregeln, die definieren, wie eingehender ('ingress' - Eingangsdatenverkehr) und abgehender
Datenverkehr ('egress' - Ausgangsdatenverkehr) an bzw. von sowohl öffentlichen als auch privaten Schnittstellen einer virtuellen Serverinstanz gehandhabt wird. Die Regeln, die Sie einer Sicherheitsgruppe hinzufügen, werden als *Sicherheitsgruppenregeln* bezeichnet.
{:shortdesc}

* Sie können Sicherheitsgruppen den öffentlichen und/oder privaten Netzschnittstellen eines einzelnen virtuellen Servers oder mehrerer virtueller Serverinstanzen zuordnen.
* Sie können Sicherheitsgruppen zuordnen, die von IBM bereitgestellt wurden oder die Sie selbst erstellt haben.
* Wenn eine Sicherheitsgruppe für eine Netzkomponente einer virtuellen Serverinstanz angewendet wird, wird der gesamte Datenverkehr zu und von dieser Netzkomponente blockiert, es sei denn, er wird durch eine Sicherheitsgruppenregel explizit zugelassen.
* Der eingehende Datenverkehr einer virtuellen Serverinstanz wird als Eingangsdatenverkehr ('ingress') bezeichnet.
* Der abgehende Datenverkehr einer virtuellen Serverinstanz wird als Ausgangsdatenverkehr ('egress') bezeichnet.

## Von IBM bereitgestellte Sicherheitsgruppen
Sie können den Netzschnittstellen Ihrer virtuellen Serverinstanzen eine beliebige der folgenden, von IBM® bereitgestellten
Sicherheitsgruppen zuordnen:

* *allow_ssh*: Diese Sicherheitsgruppe definiert IP-Regeln, die TCP-Eingangsdatenverkehr nur am SSH-Port zulassen (22/TCP).
* *allow_http*: Diese Sicherheitsgruppe definiert IP-Regeln, die Eingangsdatenverkehr nur am HTTP-Port zulassen (80/TCP).
* *allow_https*: Diese Sicherheitsgruppe definiert IP-Regeln, die TCP-Eingangsdatenverkehr nur am HTTPS-Port zulassen (443/TCP).
* *allow_outbound*: Diese Sicherheitsgruppe definiert IP-Regeln, die jeglichen Ausgangsdatenverkehr vom Server zulassen.
* *allow_all*: Diese Sicherheitsgruppe definiert IP-Regeln, die jeglichen Eingangsdatenverkehr auf allen Ports zulassen.

Im folgenden Diagramm sind virtuelle Serverinstanzen einer Reihe von Sicherheitsgruppen zugeordnet,
mit denen der Netzdatenverkehr eingeschränkt wird. Die Pfeile stellen den Datenverkehr im Netz dar. Der Anwendungsentwickler hat den Zugriff auf die verschiedenen Infrastrukturebenen wie folgt eingeschränkt:

* Der Anwendungsentwickler verfügt nur über Zugriff auf die Web-Ebene über TCP-Port 443 (https).
* Nur Instanzen der Web-Ebene verfügen über Zugriff auf die Instanzen der Anwendungsebene.
* Nur Instanzen der Anwendungsebene verfügen über Zugriff auf die Instanzen der Datenbankebene. 

![Abbildung der Sicherheitsgruppen](images/SecurityGroups.png "Abbildung des Datenverkehrs im Netz mit einer Reihe aktivierter Sicherheitsgruppen") Abbildung 1. Sicherheitsgruppen


