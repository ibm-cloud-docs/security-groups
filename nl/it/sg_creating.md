---

copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: create, rules, assign, interface, virtual server

subcollection: security-group
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}


# Creazione di gruppi di sicurezza e regole
{: #creating-security-groups}

Puoi creare un gruppo di sicurezza e le sue regole associate e assegnarlo quindi all'interfaccia di una o più istanze del server virtuale per attivare un firewall virtuale.

## Creazione di un gruppo di sicurezza
{: #creating-a-security-group-1}

Per creare un gruppo di sicurezza, completa la seguente procedura:

1. Nel [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://cloud.ibm.com/classic), seleziona **Sicurezza -> Sicurezza di rete -> Gruppi di sicurezza**.
2. Nella pagina Gruppi di sicurezza, fai clic su **Crea gruppo**.
3. Immetti un nome e una descrizione per il gruppo di sicurezza e fai di nuovo clic su **Crea gruppo**.

**Crea gruppo con una regola predefinita per consentire tutto il traffico in uscita** è selezionato per impostazione predefinita. Puoi deselezionare questo campo per creare il gruppo di sicurezza senza regole. Un gruppo di sicurezza senza regole blocca tutto il traffico (in entrata e in uscita).
{: note}

## Creazione delle regole del gruppo di sicurezza
{: #creating-security-group-rules}

Per creare una regola del gruppo di sicurezza, completa la seguente procedura:

1. Nel [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://cloud.ibm.com/classic), seleziona **Sicurezza > Sicurezza di rete > Gruppi di sicurezza**.
2. Nella pagina Gruppi di sicurezza, fai clic sul nome di un gruppo di sicurezza per aprire la pagina Dettagli e seleziona **Crea regola**.
3. Nella pagina Crea regola, immetti tutti gli attributi appropriati (come direzione, tipo IP, protocollo e le informazioni di origine/destinazione). Al termine, fai clic su **Ok**.

La selezione dei campi di destinazione o di origine facoltativi limiterà la nuova regola che viene applicata solo al traffico verso e dalla destinazione/origine specificata.  I campi di destinazione e di origine possono specificare un CIDR (Classless Inter-Domain Routing) o un gruppo di risorse.
{: note}

Un blocco CIDR facilita l'instradamento di un blocco di indirizzi IP.  Se come tipo selezioni CIDR, devi specificare un intervallo di indirizzi IP.

Se come tipo selezioni i gruppi di sicurezza, devi effettuare una selezione dall'elenco di gruppi di sicurezza esistenti. Questa selezione consente un qualsiasi indirizzo IP da un dispositivo collegato al gruppo di sicurezza selezionato. Se un server virtuale è configurato per avere più indirizzi IP, solo gli indirizzi IPv4 e IPv6 primari vengono utilizzati da queste regole del gruppo di sicurezza remote.
