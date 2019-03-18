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

# Creazione di un gruppo di sicurezza
{: #creating-a-security-group}

Crea e configura un gruppo di sicurezza personalizzato:

1. Dal tuo browser, apri il [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window} e accedi al tuo account.
2.	Seleziona la scheda **Sicurezza**.
3. Da **Sicurezza di rete** seleziona **Gruppi di sicurezza**.
4.	Fai clic su **Crea gruppo +**.
5.	Immetti un nome per il gruppo di sicurezza e facoltativamente una descrizione.
6. Fai clic su **Crea gruppo**.

![Crea un gruppo di sicurezza](./images/create_sg.jpg)

Nota che la casella **Crea un gruppo con un'impostazione predefinita…** non è spuntata. Questo significa che non sarà creata alcuna regola in uscita per questo oggetto del gruppo di sicurezza. Di conseguenza, a meno che non vengano creati altri oggetti del gruppo di sicurezza o regole in uscita, saranno permesse solo le richieste in entrata (come SSH e ICMP) e i flussi di traffico (in uscita) o le risposte correlati.

## Passo successivo...
[Crea una regola](/docs/infrastructure/security-groups?topic=security-groups-creating-a-new-rule) per consentire le richieste in entrata (SSH e ICMP) e i relativi flussi di traffico (in uscita).  
