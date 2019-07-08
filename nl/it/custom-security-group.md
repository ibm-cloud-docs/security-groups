---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: create, manage, custom, instance, assign, edit

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# Creazione e gestione di un gruppo di sicurezza personalizzato
{: #creating-and-managing-a-custom-security-group}

In questa esercitazione imparerai come creare, assegnare le istanze a e modificare un gruppo di sicurezza personalizzato.

![Gruppo di sicurezza personalizzato](./images/goal.jpg)

## Cosa ti serve
{: #what-you-ll-need-3}

Per questo esempio utilizzerai i seguenti oggetti ed elementi:

| Nome risorsa  | Sistema operativo | Tipo | Ubicazione/DC | IP/Sottorete |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| Non applicabile/Qualsiasi | 10.0.0.0/16 |
| allow_icmp | Non applicabile  | Gruppo di sicurezza | Non applicabile/Qualsiasi | 0.0.0.0/0 |
| allow_ssh | Non applicabile | Gruppo di sicurezza | Non applicabile/Qualsiasi | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Istanza del server virtuale | Dallas 10 Pod 01 | 10.0.0.21 |
|jpmongevsi4.testing.com | Ubuntu 16.04 | Istanza del server virtuale |	Dallas 10 Pod 01	| 10.0.2.219 |


Nota che questa esercitazione utilizza un account/rete privata CPA, tuttavia, per scopi pratici i gruppi di sicurezza si comportano nello stesso modo negli account CPA e in quelli regolari. Le sottoreti 10.0.0.0/24 e 10.0.2.0/24 appartengono alla stessa rete privata CPA, che dovrebbe essere l'equivalente di disporre di un account regolare con due o più VSI collegate alla stessa VLAN/sottorete privata.


## Cosa otterrai
{: #what-you-ll-accomplish-3}

In questa esercitazione imparerai come...

Attività  | Descrizione
------------- | -------------
[Creare un gruppo di sicurezza](/docs/infrastructure/security-groups?topic=security-groups-creating-a-security-group) | Crea e configura un gruppo di sicurezza personalizzato, invece di utilizzarne uno predefinito dalla piattaforma IBM© Cloud.
[Creare una regola](/docs/infrastructure/security-groups?topic=security-groups-creating-a-new-rule) | Crea una regola per consentire le richieste in entrata (SSH e ICMP) e i relativi flussi di traffico (in uscita).
[Assegnare le istanze al gruppo di sicurezza](/docs/infrastructure/security-groups?topic=security-groups-assigning-instances-to-the-security-group) | Assegna gli oggetti del gruppo di sicurezza alle istanze utilizzando il menu Sicurezza o Dispositivo.
[Modificare un gruppo di sicurezza e le relative regole](/docs/infrastructure/security-groups?topic=security-groups-editing-a-security-group) | Modifica i parametri dell'oggetto di sicurezza e le relative regole.
