---



copyright:
  years: 2017
lastupdated: "2017-08-08"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Informationen zu Sicherheitsgruppen (Beta) 

## Definition einer Sicherheitsgruppe 
Eine *Sicherheitsgruppe* ist eine Gruppe von IP-Filterregeln, die definieren, wie eingehender ('ingress' - Eingangsdatenverkehr) und abgehender
Datenverkehr ('egress' - Ausgangsdatenverkehr) an bzw. von sowohl öffentlichen als auch privaten Schnittstellen einer virtuellen Serverinstanz gehandhabt wird.
Die Regeln, die Sie einer Sicherheitsgruppe hinzufügen, werden als *Sicherheitsgruppenregeln* bezeichnet.
{:shortdesc}

* Sie können Sicherheitsgruppen einem einzelnen virtuellen Server oder mehreren virtuellen Serverinstanzen zuordnen.

* Sie können Sicherheitsgruppen zuordnen, die von IBM bereitgestellt wurden oder die Sie selbst erstellt haben. 
* Der eingehende Datenverkehr einer virtuellen Serverinstanz wird als Eingangsdatenverkehr ('ingress') bezeichnet. 
* Der abgehende Datenverkehr einer virtuellen Serverinstanz wird als Ausgangsdatenverkehr ('egress') bezeichnet. 

## Von IBM bereitgestellte Sicherheitsgruppen 
Sie können den Netzschnittstellen Ihrer virtuellen Serverinstanzen eine beliebige der folgenden, von IBM® bereitgestellten
Sicherheitsgruppen zuordnen:


* *allow_ssh*: Diese Sicherheitsgruppe definiert IP-Regeln, die TCP-Eingangsdatenverkehr nur am SSH-Port zulassen (22/TCP). Jeglicher andere Datenverkehr wird geblockt. 
* *allow_http*: Diese Sicherheitsgruppe definiert IP-Regeln, die Eingangsdatenverkehr nur am HTTP-Port zulassen (80/TCP). Jeglicher andere Datenverkehr wird geblockt. 
* *allow_https*: Diese Sicherheitsgruppe definiert IP-Regeln, die TCP-Eingangsdatenverkehr nur am HTTPS-Port zulassen
(443/TCP). Jeglicher andere Datenverkehr wird geblockt. 
* *allow_outbound*: Diese Sicherheitsgruppe definiert IP-Regeln, die jeglichen Ausgangsdatenverkehr vom Server zulassen. 
* *allow_all*: Diese Sicherheitsgruppe definiert IP-Regeln, die jeglichen Eingangsdatenverkehr auf allen Ports zulassen. 

**Hinweis:** Jede vordefinierte Sicherheitsgruppe enthält eine einzelne Sicherheitsgruppenregel. 
