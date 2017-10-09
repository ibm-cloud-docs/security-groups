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

# API-Referenz der Sicherheitsgruppe
{: #api-reference} 

Die SoftLayer&reg;-API (API - Application Programming Interface) ist die Entwicklungsschnittstelle, über die Entwickler und
Systemadministratoren direkt mit dem Back-End-System von SoftLayer interagieren können.
{:shortdesc}

Die SoftLayer-API (SLAPI) stützt viele Funktionen im Kundenportal; dies bedeutet in der Regel, dass eine Interaktion, die im
Kundenportal möglich ist, auch in der API ausgeführt werden kann. Da Sie in der API programmgestützt mit allen Teilen der SoftLayer-Umgebung interagieren können,
kann die API zum Automatisieren von Tasks verwendet werden. Zum Beispiel können Sie mithilfe der API *SoftLayer_Virtual_Guest/createObject* eine virtuelle Serverinstanz bereitstellen,
für die eine Sicherheitsgruppe aktiviert ist.

Die SoftLayer-API ist ein Remote Procedure Call-System. Bei jedem Aufruf werden Daten an einen API-Endpunkt gesendet und im
Gegenzug strukturierte Daten erhalten. Das Format, das zum Senden und Empfangen von Daten mithilfe der API verwendet wird, hängt von der von Ihnen gewählten Implementierung der API ab. 

Weitere Informationen zur SoftLayer-API, zum virtuellen Server und zu den APIs der Sicherheitsgruppen finden Sie in den folgenden
Ressourcen im SoftLayer Development Network:
* [SoftLayer-API - Übersicht ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://sldn.softlayer.com/article/softlayer-api-overview){: new_window} 
* [Einführung in die SoftLayer-API ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](http://sldn.softlayer.com/article/getting-started){: new_window}
* [API *SoftLayer_Virtual_Guest/createObject* ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest/createObject){: new_window}
* [API *SoftLayer_Network_SecurityGroup* ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://sldn.softlayer.com/reference/services/SoftLayer_Network_SecurityGroup){: new_window}
* [API *SoftLayer_Virtual_Guest_Network_Component* ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest_Network_Component){: new_window}

Für die Interaktion mit Sicherheitsgruppen können Sie auch SoftLayer API Python Client verwenden. Weitere Informationen finden Sie über die folgenden Links:
* [SoftLayer API Python Client: Mit virtuellen Servern arbeiten ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](http://softlayer-python.readthedocs.io/en/latest/cli/vs.html){: new_window}
* [Python-Beispiele für softlayer_network_securitygroup ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://softlayer.github.io/classes/softlayer_network_securitygroup/){: new_window}
