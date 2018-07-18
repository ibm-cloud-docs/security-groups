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

# Creazione e gestione di un gruppo di sicurezza personalizzato 
In questa esercitazione imparerai come creare, assegnare le istanze a e modificare un gruppo di sicurezza personalizzato. 

![Gruppo di sicurezza personalizzato](./images/goal.jpg)

## Cosa ti serve
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

In questa esercitazione imparerai come...

Attività | Descrizione 
------------- | -------------
[Creare un gruppo di sicurezza](csg_create.html) | Crea e configura un gruppo di sicurezza personalizzato, invece di utilizzarne uno predefinito dalla piattaforma IBM Cloud.
[Creare una regola](csg_rule.html)  | Crea una regola per consentire le richieste in entrata (SSH e ICMP) e i relativi flussi di traffico (in uscita).
[Assegnare le istanze al gruppo di sicurezza](csg_assign_instances.html) | Assegna gli oggetti del gruppo di sicurezza alle istanze utilizzando il menu Sicurezza o Dispositivo.
[Modificare un gruppo di sicurezza e le relative regole](csg_edit.html) | Modifica i parametri dell'oggetto di sicurezza e le relative regole.
