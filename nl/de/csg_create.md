---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: create, configure, configuration, custom

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:note: .note}
{:important: .important}
{:tip: .tip}
{:table: .aria-labeledby="caption"}

# Sicherheitsgruppe erstellen
{: #creating-a-security-group}

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
{: #next-step-2}

[Eine Regel erstellen](/docs/infrastructure/security-groups?topic=security-groups-creating-a-new-rule), um eingehende Anforderungen (SSH & ICMP) und ihre zugehörigen (abgehenden) Datenflüsse zuzulassen.  
