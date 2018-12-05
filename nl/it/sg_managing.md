---



copyright:
  years: 2017
lastupdated: "2018-11-10"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gestione dei gruppi di sicurezza
{: #managing-sg}

Puoi gestire i gruppi di sicurezza utilizzando la pagina Gruppi di sicurezza o la pagina Dettagli del dispositivo nel Portale del cliente.
{:shortdesc}

## Gestione dei gruppi di sicurezza dalla pagina Gruppi di sicurezza

Per gestire i gruppi di sicurezza dalla pagina Gruppi di sicurezza, completa la seguente procedura:
{:shortdesc}

1. Dal [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/), seleziona **Sicurezza -> Sicurezza di rete -> Gruppi di sicurezza**.
2. Nella sezione Gruppi di sicurezza, puoi completare diverse attività di gestione.
     * Visualizzare un elenco di gruppi di sicurezza.
     * Creare un gruppo.
     * Modificare le informazioni sul gruppo.
     * Duplicare un gruppo.
     * Eliminare un gruppo.
     
## Gestione delle regole del gruppo di sicurezza dalla pagina Gruppi di sicurezza

Per gestire le regole del gruppo di sicurezza dalla pagina Gruppi di sicurezza, completa la seguente procedura:
{:shortdesc}

1. Dal [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/), seleziona **Sicurezza -> Sicurezza di rete -> Gruppi di sicurezza**.
2. Fai clic sul nome di un gruppo di sicurezza per aprire la pagina Dettagli.
3. Dalla pagina Dettagli del gruppo di sicurezza, puoi completare diverse attività di gestione.
     * Visualizzare un elenco di regole definite per il gruppo di sicurezza.
     * Creare nuove regole.
     * Modificare una regola.
     * Eliminare una regola.
     * Visualizzare le istanze del server virtuale e le interfacce associate che vengono assegnate al gruppo di sicurezza.
     
**Suggerimento:** se elimini l'ultima regola in un gruppo di sicurezza, tale gruppo di sicurezza non consentirà alcun traffico in entrata o in uscita.
     
## Gestione dei gruppi di sicurezza dalla pagina Dettagli del dispositivo

Per gestire i gruppi di sicurezza dalla pagina Dettagli del dispositivo, completa la seguente procedura:
{:shortdesc}

1. Dal [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/), seleziona **Dispositivi -> Elenco dispositivi**.
2. Seleziona il nome dispositivo del server virtuale che hai ordinato. Viene visualizzata la pagina Dettagli del dispositivo.
3. Dalla pagina Dettagli del dispositivo, verifica di essere sulla scheda **Configurazione**.
4. Nella sezione Gruppi di sicurezza, puoi completare diverse attività di gestione.
     * Visualizzare gruppi di sicurezza e regole.
     * Assegnare i gruppi di sicurezza a un'interfaccia di rete di un'istanza del server virtuale.
     * Rimuovere i gruppi di sicurezza da un'interfaccia di rete di un'istanza del server virtuale.
     
     **Importante** : la prima volta che assegni un gruppo di sicurezza esistente a un'interfaccia di rete (pubblica o privata), è richiesto un riavvio per ciascuna interfaccia.  Tuttavia, se le interfacce pubbliche e private sono state assegnate al gruppo di sicurezza contemporaneamente, è richiesto un solo riavvio.  Dopo il riavvio, le modifiche vengono applicate automaticamente.
     
     Quando assegni un nuovo gruppo di sicurezza, esso impedisce di stabilire nuove connessioni in base alle definizioni delle regole del gruppo di sicurezza. Tuttavia, le connessioni socket esistenti non vengono terminate.

     **Suggerimento**: se rimuovi l'ultimo gruppo di sicurezza assegnato a un'istanza del server virtuale, il traffico del server virtuale non viene più limitato dai gruppi di sicurezza. Non esiste più un firewall del gruppo di sicurezza.
     
6. Dopo aver apportato le modifiche, fai clic su **Salva**.
