---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"

keywords: add, order, group

subcollection: security-groups


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

# Aggiunta di gruppo di sicurezza predefinito durante l'ordine
{: #adding-a-pre-defined-security-group-during-ordering}

Questa procedura dettagliata ti mostra come aggiungere gruppi di sicurezza predefiniti o esistenti alle istanze durante il processo di ordine.

Puoi utilizzare i gruppi di sicurezza per applicare una serie di regole di filtro IP che definiscono come gestire il traffico in entrata e in uscita alle interfacce pubbliche e private di un'istanza del server virtuale.

![Gruppo di sicurezza personalizzato](./images/goal2.jpg)

## Cosa ti serve
{: #what-you-ll-need-2}

Per questo esempio utilizzerai i seguenti oggetti ed elementi:

| Nome risorsa  | Sistema operativo | Tipo | Ubicazione/DC | IP/Sottorete |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| allow_ssh1 | Non applicabile  | Gruppo di sicurezza | Non applicabile/Qualsiasi | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Istanza del server virtuale | Dallas 10 Pod 01 | 10.0.0.21 |
|jpmongevsi4.testing.com | Ubuntu 16.04 | Istanza del server virtuale |	Dallas 10 Pod 01	| 10.0.2.219 |

## Ordina un gruppo di sicurezza
{: #order-a-security-group}

Per ordinare un'istanza del server virtuale e assegnare un gruppo di sicurezza, esegui la seguente procedura:

1. Dal tuo browser, apri il [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://cloud.ibm.com/classic) e accedi al tuo account.
2. Individua la sezione **Ordine** e fai clic su **Dispositivi**.
3. Nella pagina Dispositivi, fai clic su **Oraria** o **Mensile** per una delle offerte del server virtuale.
4. Nella pagina Configura ordine server cloud, devi selezionare un data center che supporta i gruppi di sicurezza.
5. Completa tutte le altre informazioni necessarie e fai clic su **Aggiungi all'ordine**. Viene visualizzata la pagina di verifica.
6. Conferma le seguenti informazioni per la VSI:

	* Ubicazione
	* Specifiche
	* Opzioni della porta di rete.

7. Da **Configura gruppi di sicurezza**, seleziona il gruppo di sicurezza desiderato da applicare. Le regole associate a ogni gruppo di sicurezza possono essere visualizzate facendo clic sul link **Visualizza regole**.

	![Gruppo di sicurezza personalizzato](./images/sgs.jpg)

	Puoi selezionare qualsiasi gruppo di sicurezza predefinito da applicare alle interfacce private o pubbliche sul server virtuale.

8. Specifica il nome dell'istanza.
9. Spunta la casella dei termini del servizio cloud e degli accordi di servizio di terze parti se applicabile.
10. Infine, fai clic su **Inoltra ordine**.
