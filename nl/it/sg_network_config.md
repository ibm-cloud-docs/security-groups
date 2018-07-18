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
| AMS01             |
| AMS03             |
| CHE01             |
| DAL01             |
| DAL05             |
| DAL06             |
| DAL09             |
| DAL10             |
| DAL12             |
| DAL13             |
| FRA02             |
| FRA04             |
| FRA05             |
| HKG02             |
| HOU02             |
| LON02             |
| LON04             |
| LON06             |
| MEL01             |
| MEX01             |
| MIL01             |
| MON01             |
| OSL01             |
| PAR01             |
| SAO01             |
| SEA01             |
| SEO01             |
| SJC01             |
| SJC03             |
| SJC04             |
| SNG01             |
| SYD01             |
| SYD04             |
| TOK02             |
| TOR01             |
| WDC01             |
| WDC04             |
| WDC06             |
| WDC07             |
{: caption="Tabella 2. Data center che supportano i gruppi di sicurezza" caption-side="top"} 
