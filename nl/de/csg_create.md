---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Sicherheitsgruppe erstellen
Erstellen und konfigurieren Sie eine angepasste Sicherheitsgruppe. 

1. Rufen Sie in Ihrem Browser das [Kundenportal ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} auf und melden Sie sich bei Ihrem Konto an. 
2.	Wählen Sie die Registerkarte **Sicherheit** aus. 
3. Wählen Sie unter **Netzsicherheit** den Eintrag **Sicherheitsgruppen** aus. 
4.	Klicken Sie auf **Gruppe erstellen +**. 
5.	Geben Sie einen Namen für die Sicherheitsgruppe und optional eine Beschreibung ein. 
6. Klicken Sie auf **Gruppe erstellen**. 

![Sicherheitsgruppe erstellen](./images/create_sg.jpg)

Beachten Sie, dass das Kontrollkästchen **Gruppe mit einem Standardwert erstellen…** nicht markiert ist. Das bedeutet, dass keine abgehende Regel für dieses Sicherheitsgruppenobjekt erstellt wird. Folglich werden auch nur eingehende Anforderungen (wie SSH und ICMP) sowie ihre zugehörigen Datenflüsse zugelassen, es sei denn, andere abgehende Regeln oder Sicherheitsgruppenobjekte werden erstellt. 

## Nächster Schritt ...
[Eine Regel erstellen](csg_rule.html), um eingehende Anforderungen (SSH & ICMP) und ihre zugehörigen (abgehenden) Datenflüsse zuzulassen.   
