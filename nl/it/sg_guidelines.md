---



copyright:
  years: 2017
lastupdated: "2018-11-10"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Linee guida per i gruppi di sicurezza
{: #security-groups-guidelines}

Quando lavori con i gruppi di sicurezza, considera le seguenti linee guida:

## Regole

* Ogni gruppo di sicurezza definisce diverse serie di regole della rete che definiscono il traffico in entrata e in uscita per un'istanza del server virtuale. Puoi specificare le regole per IPv4 e IPv6.
* Quando si crea un nuovo gruppo di sicurezza utilizzando l'interfaccia Portale del cliente, il comportamento predefinito è quello di creare una singola regola che consente tutto il traffico in uscita dall'istanza del server virtuale. Per creare il gruppo di sicurezza senza regole, devi deselezionare la casella di spunta "Crea gruppo con una regola predefinita per consentire tutto il traffico in uscita". Un gruppo di sicurezza senza regole blocca tutto il traffico (in entrata e in uscita).
* Per consentire il traffico in entrata e/o il traffico in uscita, devi aggiungere almeno un gruppo di sicurezza che includa le regole che consentono il traffico.
* Le regole del gruppo di sicurezza possono essere solo permissive. Il traffico è bloccato per impostazione predefinita.
* Gli utenti con il privilegio Gestisci gruppi di sicurezza possono aggiungere, modificare o eliminare le regole in un gruppo di sicurezza.
* Le modifiche alle regole del gruppo di sicurezza vengono applicate automaticamente e possono essere effettuate in qualsiasi momento.
* L'ordine delle regole all'interno di un gruppo di sicurezza non ha rilevanza. La priorità spetta sempre alla regola meno restrittiva.
* Le regole sono con stato. Le connessioni stabilite prima di una modifica al gruppo di sicurezza non saranno modificate. Le nuove connessioni si atterranno alle regole esistenti al momento in cui viene stabilita la connettività.
* I gruppi di sicurezza non sovrascrivono i firewall del sistema operativo sul server virtuale. Se nel sistema operativo esiste un firewall più restrittivo rispetto a quanto applicato dai gruppi di sicurezza, vengono ancora applicate le regole del sistema operativo.
* Se il tuo server virtuale deve accedere a servizi interni, come un server di aggiornamento, un NAS (Network Attached Storage) o un monitoraggio avanzato, assicurati che le regole del gruppo di sicurezza soddisfino il traffico per i servizi interni. Per ulteriori informazioni, vedi [What IP ranges do I allow through the firewall](/docs/infrastructure/hardware-firewall-dedicated?topic=hardware-firewall-dedicated-ibm-cloud-ip-ranges).

## Interfacce

* Un gruppo di sicurezza può essere applicato a una rete privata, una rete pubblica o entrambi i tipi di interfaccia di rete.
* Puoi collegare uno o più gruppi di sicurezza all'elenco di gruppi di sicurezza assegnati a un'interfaccia di rete. Le regole di ciascun gruppo di sicurezza vengono applicate alle istanze del server virtuale associato.
* La prima volta che assegni un gruppo di sicurezza esistente a un'interfaccia di rete (pubblica o privata), è richiesto un riavvio per ciascuna interfaccia.  Tuttavia, se le interfacce pubbliche e private sono state assegnate al gruppo di sicurezza contemporaneamente, è richiesto un solo riavvio.  Dopo il riavvio, le modifiche vengono applicate automaticamente.

## Accesso

* Tutti gli utenti di un account possono leggere, collegare e scollegare i gruppi di sicurezza nelle istanze del server virtuale a cui hanno accesso. Solo gli utenti che dispongono del privilegio Gestisci gruppi di sicurezza in Autorizzazioni di rete possono creare, aggiornare ed eliminare i gruppi di sicurezza.
* Non puoi assegnare gruppi di sicurezza a server bare metal.

## Eliminazione

* Non puoi eliminare un gruppo di sicurezza assegnato a una o più istanze del server virtuale in esecuzione.
* Non puoi eliminare un gruppo di sicurezza a cui fa riferimento un altro gruppo di sicurezza in una delle sue regole.
