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

## Gruppi di sicurezza forniti da IBM
Puoi assegnare uno dei seguenti gruppi di sicurezza forniti da IBM® alle interfacce di
rete delle tue istanze del server virtuale:

* *allow_ssh*: questo gruppo di sicurezza definisce le regole IP che consentono il traffico TCP in ingresso solo sulla porta SSH (22/TCP).
* *allow_http*: questo gruppo di sicurezza definisce le regole IP che consentono il traffico in ingresso solo sulla porta HTTP (80/TCP).
* *allow_https*: questo gruppo di sicurezza definisce le regole IP che consentono il traffico TCP in ingresso solo sulla porta HTTPS (443/TCP).
* *allow_outbound*: questo gruppo di sicurezza definisce le regole IP che consentono tutto il traffico in uscita dal server.
* *allow_all*: questo gruppo di sicurezza definisce le regole IP che consentono tutto il traffico in ingresso su tutte le porte.

Nel seguente diagramma, le istanze del server virtuale sono associate
a una serie di gruppi di sicurezza per limitare il traffico di rete. Le frecce rappresentano il flusso del traffico di rete. Lo sviluppatore dell'applicazione ha accesso limitato ali vari livelli dell'infrastruttura, nel seguente modo:

* Lo sviluppatore dell'applicazione può accedere solo a livello web nella porta TCP 443 (https).
* Solo le istanze a livello web possono accedere alle istanze a livello dell'applicazione.
* Solo le istanze a livello dell'applicazione possono accedere alle istanze a livello database. 

![Immagine gruppo di sicurezza](images/SecurityGroups.png "L'immagine mostra il flusso del traffico di rete con una serie di gruppi di sicurezza abilitati") Figura 1. Immagine gruppo di sicurezza


