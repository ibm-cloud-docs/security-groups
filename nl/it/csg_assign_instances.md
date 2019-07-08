---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"

keywords: assign, instance

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:note: .note}
{:important: .important}
{:tip: .tip}
{:table: .aria-labeledby="caption"}

# Assegnazione di istanze al gruppo di sicurezza
{: #assigning-instances-to-the-security-group}

Puoi assegnare gli oggetti del gruppo di sicurezza alle istanze in due modi:

## Utilizzo del menu Sicurezza
{: #using-the-security-menu}

1. Dalla scheda **Sicurezza** nel [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window}, in **Sicurezza di rete** seleziona **Gruppi di sicurezza**.
2. Fai clic sull'icona ![Icona Altro](./images/more_icon.jpg) dell'oggetto del gruppo di sicurezza a cui vuoi assegnare le istanze, poi seleziona **Gestisci istanze**.
3. Seleziona l'istanza e l'interfaccia da applicare al gruppo di sicurezza.

	![Istanza menu Sicurezza](./images/security_assign.jpg)

	Nella figura, il gruppo di sicurezza "allow_icmp" (creato nel [primo passo](/docs/infrastructure/security-groups?topic=security-groups-creating-a-security-group)) viene applicato all'interfaccia privata (`10.0.2.219`) di "jpmongevsi4".

	Nota in che modo il numero di **Istanze collegate** viene aumentato da `0` a `1`.

4. Fare clic su **Salva** per applicare le modifiche.

5. Riavvia la tua istanza.

	Questo è un passo unico per ogni interfaccia di rete per le istanze non create con un gruppo di sicurezza.
  {: note}

## Utilizzo del menu Dispositivi
{: #using-the-devices-menu}

1. Dalla scheda **Dispositivi** nel [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window}, seleziona **Elenco dispositivi**.
2. Fai clic sul nome dell'istanza in cui vuoi applicare l'oggetto del gruppo di sicurezza.
3. Seleziona **Modifica** e contrassegna l'oggetto del gruppo di sicurezza che vuoi associare all'istanza.

	![Istanza menu Dispositivo](./images/device_assign.jpg)

	Questa figura mostra l'oggetto del gruppo di sicurezza "allow_icmp" che sta venendo assegnato all'interfaccia privata dell'istanza jpmongevsi4.
4. Fare clic su **Salva** per applicare le modifiche.

5. Riavvia l'istanza.

	Questo è un passo unico per ogoni interfaccia di rete per le istanze non create con un gruppo di sicurezza.
  {: note}

## Passo successivo...
{: #next-step-1}

[Modifica il gruppo di sicurezza](/docs/infrastructure/security-groups?topic=security-groups-editing-a-security-group) per modificarne i parametri.  
