---



copyright:
  years: 2017
lastupdated: "2018-11-10"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Bereitstellung von Umgebungen mit Schemas automatisieren
Führen Sie die folgenden Schritte aus, um eingehende Anforderungen (SSH & ICMP) und ihre zugehörigen (abgehenden) Datenflüsse zuzulassen:

1. Wählen Sie die Registerkarte **Regeln** im [Kundenportal ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://cloud.ibm.com/classic){: new_window} aus.
2.	Klicken Sie auf **Regel erstellen**.
3.	Geben Sie ggf. die Richtung, den IP-Typ, das Protokoll, den Portbereich, den Typ, den Code und die Quelle der Regel an (basierend auf der Protokollauswahl). 

	Wenn Sie nicht eine andere Sicherheitsgruppe als Quelle verwenden, belassen Sie **Quellentyp** bei 'CIDR-Block'.
	
	![Regel erstellen](rule_sg.jpg)
	
	In der Abbildung oben ist **All ICMP** als Protokoll ausgewählt, was bedeutet, dass alle ICMP-Typen und -Codes zulässig sind. Außerdem wird das Feld 'Quelle' leer gelassen; verwendet wird der Standardwert `0.0.0.0/0`, das Äquivalent zu einer beliebigen IP-Adresse oder einem beliebigen Teilnetz.

4.	Klicken Sie auf **OK**, um den Vorgang zu beenden.
