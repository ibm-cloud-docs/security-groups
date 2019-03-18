---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Introduzione ai gruppi di sicurezza
{: #getting-started-with-security-groups}

Puoi utilizzare i gruppi di sicurezza per applicare una serie di regole di filtro IP che definiscono come gestire il traffico in entrata e in uscita alle interfacce pubbliche e private di un'istanza del server virtuale.
{:shortdesc}

Per iniziare, ordina una VSI (Virtual Server Instance) e assegna un gruppo di sicurezza.
 
1. Dal tuo browser, apri il [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/) e accedi al tuo account.
2. Individua la sezione **Ordine** e fai clic su **Dispositivi**.
3. Nella pagina Dispositivi, fai clic su **Oraria** o **Mensile** per una delle offerte del server virtuale.
4. Nella pagina dell'ordine **Configura il tuo server cloud**, devi selezionare un data center che supporta i gruppi di sicurezza.
5. Completa tutte le altre informazioni necessarie e fai clic su **Aggiungi all'ordine**. Viene visualizzata la pagina di verifica.
6. Completa le informazioni in **Configura gruppi di sicurezza**.
7. Puoi selezionare qualsiasi gruppo di sicurezza predefinito da applicare alle interfacce private o pubbliche sul server virtuale.
8. Infine, fai clic su **Inoltra ordine**.

## Soluzioni e casi di utilizzo
Le seguenti sezioni descrivono alcuni complessi scenari di sicurezza della rete che potresti incontrare e che possono essere risolti utilizzando i gruppi di sicurezza.

### Sicurezza dall'inizio
**Scenario di sicurezza:** i clienti vogliono proteggere il proprio server virtuale come ne viene eseguito il provisioning. Vogliono il controllo completo sul traffico che passa per il server dal momento in cui ne è stato eseguito il provisioning.

**Soluzione:** utilizza i gruppi di sicurezza al momento dell'ordine del server virtuale. In questo modo, il tuo server viene protetto dal momento del suo provisioning.

### Firewall a livello dell'istanza economicamente vantaggioso
**Scenario di sicurezza:** i clienti vogliono avere il controllo granulare sul traffico a un livello dell'istanza (a parte la protezione firewall al livello della rete), ma allo stesso tempo, i costi di un firewall hardware condiviso (che è un'offerta a più tenant a livello dell'istanza di IBM) possono essere aggiunti velocemente se il cliente ha bisogno di proteggere più server in diversi data center. 

**Soluzione:** non c'è alcun costo aggiuntivo per l'utilizzo della funzione dei gruppi di sicurezza. Utilizza i gruppi di sicurezza per tutti i server virtuali che hanno bisogno di protezione in uno qualsiasi dei nostri data center globali.

### Firewall facilmente gestibile e scalabile globalmente
**Scenario di sicurezza:** i clienti vogliono evitare la configurazione delle regole del firewall su ogni server separatamente. Invece, vogliono una soluzione firewall facilmente gestibile che suddivide i server in data center globali differenti.

**Soluzione:** definisci `N` gruppi di sicurezza per `N` tipi di server differenti nel tuo carico di lavoro cloud. Gestisci tutte le regole di un gruppo di sicurezza in un solo posto. Gestisci le associazioni del gruppo di sicurezza in modo appropriato con i server virtuali.
