---



copyright:
  years: 2017
lastupdated: "2017-04-27"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# Creazione di gruppi di sicurezza e regole 
{: #creating-security-groups}

Puoi creare un gruppo di sicurezza e le sue regole associate e assegnarlo quindi all'interfaccia di una o più istanze del server virtuale per attivare un firewall virtuale.
{:shortdesc}

## Creazione di un gruppo di sicurezza

Per creare un gruppo di sicurezza, completa la seguente procedura:
{:shortdesc}
 
1. Nel [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/), seleziona **Sicurezza -> Sicurezza di rete -> Gruppi di sicurezza**.
2. Nella pagina Gruppi di sicurezza, fai clic su **Crea gruppo**.
3. Immetti un nome e una descrizione per il gruppo di sicurezza e fai di nuovo clic su **Crea gruppo**.

**Nota:** l'opzione "Crea gruppo con una regola predefinita per consentire tutto il traffico in uscita" è selezionata per impostazione predefinita. Puoi deselezionare questo campo per creare il gruppo di sicurezza senza regole. Un gruppo di sicurezza senza regole blocca tutto il traffico (in entrata e in uscita).

## Creazione delle regole del gruppo di sicurezza

Per creare una regola del gruppo di sicurezza, completa la seguente procedura:
{:shortdesc}

1. Nel [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/), seleziona **Sicurezza -> Sicurezza di rete -> Gruppi di sicurezza**.
2. Nella pagina Gruppi di sicurezza, fai clic sul nome di un gruppo di sicurezza per aprire la pagina Dettagli.
3. Nella pagina dei dettagli del gruppo di sicurezza, immetti tutte le azioni appropriate (come direzione, tipo IP, protocollo e informazioni di origine/destinazione. Al termine, fai clic su **Crea regola**.

**Nota**: per i campi di origine e di destinazione, puoi specificare il blocco CIDR (Classless Inter-Domain Routing) o il gruppo di sicurezza. 

Un blocco CIDR facilita l'instradamento di un blocco di indirizzi IP.  Se come tipo selezioni CIDR, devi specificare un intervallo di indirizzi IP. 

Se come tipo selezioni i gruppi di sicurezza, devi effettuare una selezione dall'elenco di gruppi di sicurezza esistenti. Questa selezione consente un qualsiasi indirizzo IP da un dispositivo collegato al gruppo di sicurezza selezionato. Se un server virtuale è configurato per avere più indirizzi IP, solo gli indirizzi IPv4 e IPv6 primari vengono utilizzati da queste regole del gruppo di sicurezza remote.
