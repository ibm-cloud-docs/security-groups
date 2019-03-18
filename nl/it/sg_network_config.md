---



copyright:
  years: 2017
lastupdated: "2018-11-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Configurazioni di reti esistenti e gruppi di sicurezza
{: #existing-network-configurations-and-security-groups}

Un gruppo di sicurezza incrementa qualsiasi configurazione di rete esistente. Pertanto, un gruppo di sicurezza non può estendersi su reti che non possono
comunicare tra loro. 
{:shortdesc}

Se le istanze del server virtuale non riescono a comunicare tra di loro, aggiungerle a un gruppo di sicurezza non modifica
tale comportamento. I gateway devono consentire il traffico definito dai gruppi di sicurezza selezionati.

Se il tuo account è abilitato per l'indirizzamento privato personalizzato (CPA) e per i gruppi di sicurezza, tieni presente che i gruppi di sicurezza sono applicabili a livello di account e non a livello di rete. I gruppi di sicurezza sono definiti da indirizzi IP, non da reti private.

I gruppi di sicurezza sono disponibili in tutti i data center con il provisioning della VSI.
