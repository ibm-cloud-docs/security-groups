---



copyright:
  years: 2017
lastupdated: "2017-08-08"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Informazioni sui gruppi di sicurezza

## Cos'è un gruppo di sicurezza?
Un *gruppo di sicurezza* è una serie di regole di filtro IP che definiscono come gestire il traffico
in entrata e in uscita alle interfacce pubbliche e private di un'istanza del server virtuale. Le regole che
aggiungi a un gruppo di sicurezza sono note come *regole del gruppo di sicurezza*.
{:shortdesc}

* Puoi assegnare i gruppi di sicurezza alle interfacce di rete pubblica e/o privata di un singolo server virtuale o a più istanze del server virtuale.
* Puoi assegnare i gruppi di sicurezza forniti da IBM o creati da te.
* Quando un gruppo di sicurezza viene applicato a un componente di rete di un'istanza del server virtuale, tutto il traffico in entrata e uscita da tale componente di rete viene impedito a meno di venire esplicitamente autorizzato da una regola del gruppo di sicurezza.
* Il traffico verso un'istanza del server virtuale è indicato come traffico in ingresso.
* Il traffico da un'istanza del server virtuale è indicato come traffico in uscita.

I gruppi di sicurezza sono implementati nell'hypervisor che ospita il server virtuale.

## Gruppi di sicurezza forniti da IBM
Puoi assegnare uno dei seguenti gruppi di sicurezza forniti da IBM alle interfacce di
rete delle tue istanze del server virtuale: 

* *allow_ssh*: questo gruppo di sicurezza definisce le regole IP che consentono il traffico TCP in ingresso solo sulla porta SSH (22/TCP).
* *allow_http*: questo gruppo di sicurezza definisce le regole IP che consentono il traffico in ingresso solo sulla porta HTTP (80/TCP).
* *allow_https*: questo gruppo di sicurezza definisce le regole IP che consentono il traffico TCP in ingresso solo sulla porta HTTPS (443/TCP).
* *allow_outbound*: questo gruppo di sicurezza definisce le regole IP che consentono tutto il traffico in uscita dal server.
* *allow_all*: questo gruppo di sicurezza definisce le regole IP che consentono tutto il traffico in ingresso su tutte le porte.

## Gruppi di sicurezza e log di controllo 
Tutte le interazioni del gruppo di sicurezza sono registrate in un [log di controllo](https://console.bluemix.net/docs/customer-portal/cpmonenv.html#cp_viewacctauditlog) dell'account. Le voci del log di controllo tracciano le modifiche e quale utente ha richiesto la modifica. I log vengono scritti per le seguenti interazioni:
* Un gruppo di sicurezza viene aggiunto a o rimosso da un'interfaccia di rete del server virtuale
* Le regole di un gruppo di sicurezza vengono modificate aggiungendo, modificando o rimuovendo una regola

Per ognuna di queste interazioni, viene scritto un log per ogni oggetto interessato. Viene sempre scritto un log quando il gruppo di sicurezza viene modificato. Vengono scritti ulteriori log per ogni interfaccia di rete del server virtuale collegata al gruppo di sicurezza. Il filtro dei log di controllo in un gruppo di sicurezza specifico, mostra tutte le modifiche correlate al gruppo di sicurezza per il gruppo. Allo stesso modo, il filtro dei log in un server virtuale specifico, mostra tutte le modifiche correlate al gruppo di sicurezza per il server virtuale.

Poiché le modifiche al gruppo di sicurezza possono causare l'aggiornamento di alcuni server virtuali in background, i log di controllo possono essere utilizzati per determinare precisamente quando una modifica è diventata effettiva.  Le API del gruppo di sicurezza che generano i log di controllo restituiscono un identificativo della richiesta. Tale identificativo può essere utilizzato per correlare le chiamate API ai relativi log di controllo risultanti.

## Esempio
Nel seguente diagramma, le istanze del server virtuale sono associate
a una serie di gruppi di sicurezza per limitare il traffico di rete. Le frecce rappresentano il flusso del traffico di rete. Lo sviluppatore dell'applicazione ha accesso limitato ali vari livelli dell'infrastruttura, nel seguente modo:

* Lo sviluppatore dell'applicazione può accedere solo a livello web nella porta TCP 443 (https).
* Solo le istanze a livello web possono accedere alle istanze a livello dell'applicazione.
* Solo le istanze a livello dell'applicazione possono accedere alle istanze a livello database. 

![Immagine gruppo di sicurezza](images/SecurityGroups.png "L'immagine mostra il flusso del traffico di rete con una serie di gruppi di sicurezza abilitati") Figura 1. Immagine gruppo di sicurezza


