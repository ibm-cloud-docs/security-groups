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

# Angepasste Sicherheitsgruppe erstellen und verwalten
In diesem Lernprogramm erfahren Sie, wie Sie eine angepasste Sicherheitsgruppe erstellen, ihr Instanzen zuordnen und sie bearbeiten. 

![Angepasste Sicherheitsgruppe](./images/goal.jpg)

## Voraussetzungen
In diesem Beispiel werden die folgenden Objekte und Elemente verwendet:

| Ressourcenname  | Betriebssystem | Typ | Ort/Rechenzentrum | IP/Teilnetz |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| Nicht zutreffend/Kein | 10.0.0.0/16 |
| allow_icmp | Nicht zutreffend  | Sicherheitsgruppe | Nicht zutreffend/Kein | 0.0.0.0/0 |
| allow_ssh | Nicht zutreffend | Sicherheitsgruppe | Nicht zutreffend/Kein | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Virtuelle Serverinstanz | Dallas 10 Pod 01 | 10.0.0.21 |	
|jpmongevsi4.testing.com | Ubuntu 16.04 | Virtuelle Serverinstanz |	Dallas 10 Pod 01	| 10.0.2.219 |


Beachten Sie, dass in diesem Lernprogramm ein privates CPA-Netz bzw. ein CPA-Konto verwendet wird, aus praktischen Gründen zeigen Sicherheitsgruppen jedoch sowohl in CPA-Konten als auch in regulären Konten dasselbe Verhalten. Die Teilnetze 10.0.0.0/24 und 10.0.2.0/24 gehören zum selben privaten CPA-Netz. Dies entspricht einem regulären Konto mit zwei oder mehr VSIs, die mit demselben privaten Teilnetz/VLAN verbunden sind.


## Ergebnisse

In diesem Lernprogramm erfahren Sie. wie Sie ...

Aufgabe  | Beschreibung
------------- | -------------
[Eine Sicherheitsgruppe erstellen](csg_create.html) | Erstellen und konfigurieren Sie eine angepasste Sicherheitsgruppe, statt eine von der IBM Cloudplattform vordefinierte zu verwenden. 
[Eine Regel erstellen](csg_rule.html)  | Erstellen Sie eine Regel, um eingehende Anforderungen (SSH & ICMP) und ihre zugehörigen (abgehenden) Datenflüsse zuzulassen. 
[Instanzen zu der Sicherheitsgruppe zuordnen](csg_assign_instances.html) | Ordnen Sie Sicherheitsgruppenobjekte entweder über das Sicherheitsmenü oder das Gerätemenü zu Instanzen zu.
[Eine Sicherheitsgruppe und ihre Regeln bearbeiten](csg_edit.html) | Ändern Sie die Parameter des Sicherheitsobjekts und seine Regeln.
