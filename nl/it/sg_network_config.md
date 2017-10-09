---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Configurazioni di rete esistenti e gruppi di sicurezza 

Un gruppo di sicurezza incrementa qualsiasi configurazione di rete esistente. Pertanto, un gruppo di sicurezza non può estendersi su reti che non possono
comunicare tra loro. 
{:shortdesc}

Se le istanze del server virtuale non riescono a comunicare tra di loro, aggiungerle a un gruppo di sicurezza non modifica
tale comportamento. I gateway devono consentire il traffico definito dai gruppi di sicurezza selezionati.

Se il tuo account è abilitato per l'indirizzamento privato personalizzato (CPA) e per i gruppi di sicurezza, tieni presente che i gruppi di sicurezza sono applicabili a livello di account e non a livello di rete. I gruppi di sicurezza sono definiti da indirizzi IP, non da reti private.

I gruppi di sicurezza sono attualmente disponibili nei seguenti data center:

| Data center      | 
|:------------------|
| CHE01             |
| DAL12             |
| DAL13             |
| HKG02             |
| LON04             |
| MEL01             |
| MIL01             |
| OSL01             |
| SAO01             |
| SJC04             |
| SYD01             |
| SYD04             |
| TOR01             |
| WDC06             |
| WDC07             |
{: caption="Tabella 2. Data center che supportano i gruppi di sicurezza" caption-side="top"} 
