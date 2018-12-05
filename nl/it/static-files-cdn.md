---



copyright:
  years: 2017
lastupdated: "2018-11-10"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Accelera la distribuzione dei file statici utilizzando l'Object Storage e il CDN
Consenti le richieste in entrata (SSH e ICMP) e i relativi flussi di traffico (in uscita) eseguendo la seguente procedura:

1. Seleziona la scheda **Regole** nel [Portale del cliente ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){: new_window}.
2.	Fai clic su **Crea regola**.
3.	Specifica la direzione, il tipo di IP, il protocollo, l'intervallo di porte, il tipo, il codice e l'origine della regola quando applicabile (in base alla selezione del protocollo).

	A meno che non stai utilizzando il gruppo di sicurezza come origine, lascia il **Tipo di origine** come "blocco CIDR".

	![Crea una regola](rule_sg.jpg)

	La figura mostra **Tutti i ICMP** selezionati come protocollo, il che significa che tutti i codici e i tipi di ICMP saranno consentiti. In aggiunta, il campo Origine sta venendo lasciato vuoto, utilizzando il valore di `0.0.0.0/0` -- l'equivalente di ogni sottorete o indirizzo IP.

4.	Fai clic su **OK** per terminare.
