---



copyright:
  years: 2017, 2018
lastupdated: "2018-02-15"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Assegnazione di istanze al gruppo di sicurezza 
Puoi assegnare gli oggetti del gruppo di sicurezza alle istanze in due modi:

## Utilizzo del menu Sicurezza

1. Dalla scheda **Sicurezza** nel [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window}, in **Sicurezza di rete** seleziona **Gruppi di sicurezza**.
2. Fai clic sull'icona ![Icona Altro](./images/more_icon.jpg) dell'oggetto del gruppo di sicurezza a cui vuoi assegnare le istanze, poi seleziona **Gestisci istanze**.
3. Seleziona l'istanza e l'interfaccia da applicare al gruppo di sicurezza.

	![Istanza menu Sicurezza](./images/security_assign.jpg)

	Nella figura, il gruppo di sicurezza "allow_icmp" (creato nel [primo passo](csg_create.html)) viene applicato all'interfaccia privata (`10.0.2.219`) di "jpmongevsi4".

	Nota in che modo il numero di **Istanze collegate** viene aumentato da `0` a `1`.

4. Fare clic su **Salva** per applicare le modifiche. 

5. Riavvia la tua istanza.

	**NOTA:** questo è un passo unico per l'interfaccia di rete delle istanze non create con un gruppo di sicurezza.

## Utilizzo del menu Dispositivi

1. Dalla scheda **Dispositivi** nel [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window}, seleziona **Elenco dispositivi**.
2. Fai clic sul nome dell'istanza in cui vuoi applicare l'oggetto del gruppo di sicurezza.
3. Seleziona **Modifica** e contrassegna l'oggetto del gruppo di sicurezza che vuoi associare all'istanza.

	![Istanza menu Dispositivo](./images/device_assign.jpg)

	Questa figura mostra l'oggetto del gruppo di sicurezza "allow_icmp" che sta venendo assegnato all'interfaccia privata dell'istanza jpmongevsi4.
4. Fare clic su **Salva** per applicare le modifiche. 

5. Riavvia l'istanza.

	**NOTA:** questo è un passo unico per l'interfaccia di rete delle istanze non create con un gruppo di sicurezza.

## Passo successivo...
[Modifica il gruppo di sicurezza](csg_edit.html) per modificarne i parametri.  
