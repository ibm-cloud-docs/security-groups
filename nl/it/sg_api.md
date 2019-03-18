---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Riferimento all'API gruppo di sicurezza
{: #api-reference} 

L'API (Application Programming Interface) SoftLayer è l'interfaccia di sviluppo che fornisce agli sviluppatori e agli amministratori
di sistema un'interazione diretta con il sistema di backend SoftLayer
{:shortdesc}

L'API SoftLayer (SLAPI) potenzia molte delle funzioni del Portale del cliente, il che
in genere significa che se un'interazione è possibile nel Portale del cliente, può essere eseguita anche nell'API. Poiché puoi interagire in modo programmatico
con tutte le parti dell'ambiente SoftLayer all'interno dell'API, puoi usare l'API per automatizzare le attività. Ad esempio, puoi utilizzare
l'API *SoftLayer_Virtual_Guest/createObject* per distribuire un'istanza del server virtuale con un gruppo di sicurezza abilitato.

L'API SoftLayer è un sistema di chiamata a procedura remota. Ogni chiamata prevede l'invio di dati verso un endpoint API e la successiva ricezione dei dati
strutturati. Il formato utilizzato per inviare e ricevere dati con la SLAPI dipende da quale implementazione API scegli. 

Per ulteriori informazioni sull'API SoftLayer, sul server virtuale e sulle API del gruppo di sicurezza, consulta le seguenti risorse in SoftLayer
Development Network:
* [Panoramica dell'API SoftLayer ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://softlayer.github.io/reference/softlayerapi/){: new_window} 
* [Introduzione all'API SoftLayer ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](http://sldn.softlayer.com/article/getting-started){: new_window}
* [API *SoftLayer_Virtual_Guest/createObject* ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest/createObject){: new_window}
* [API *SoftLayer_Network_SecurityGroup* ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://sldn.softlayer.com/reference/services/SoftLayer_Network_SecurityGroup){: new_window}
* [API *SoftLayer_Virtual_Guest_Network_Component* ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest_Network_Component){: new_window}

Per interagire con i gruppi di sicurezza, puoi anche utilizzare il client Python dell'API SoftLayer. Per ulteriori informazioni, consulta i seguenti link:
* [Client Python API SoftLayer: gestione dei server virtuali ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](http://softlayer-python.readthedocs.io/en/latest/cli/vs.html){: new_window}
* [Esempi di Python per softlayer_network_securitygroup ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://softlayer.github.io/classes/softlayer_network_securitygroup/){: new_window}
