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

# Security Group API reference
{: #api-reference} 

The SoftLayer&reg; Application Programming Interface (API) is the development interface that gives developers and system administrators direct 
interaction with SoftLayer's backend system. 
{:shortdesc}

The SoftLayer API (SLAPI) powers many of the features in the Customer Portal, which 
typically means if an interaction is possible in the Customer Portal, it can also be run in the API. Because you can programmatically interact
with all portions of the SoftLayer environment within the API, you can use the API to automate tasks. For example, you can use the 
*SoftLayer_Virtual_Guest/createObject* API to deploy a virtual server instance with a security group enabled.

The SoftLayer API is a Remote Procedure Call system. Each call involves sending data towards an API endpoint and receiving structured data
in return. The format used to send and receive data with the SLAPI depends on which implementation of the API you choose. 

For more information about the SoftLayer API, virtual server, and security group APIs, see the following resources in the SoftLayer 
Development Network:
* [SoftLayer API Overview ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://softlayer.github.io/reference/softlayerapi/){: new_window} 
* [Getting Started with the SoftLayer API ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://sldn.softlayer.com/article/getting-started){: new_window}
* [*SoftLayer_Virtual_Guest/createObject* API ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest/createObject){: new_window}
* [*SoftLayer_Network_SecurityGroup* API ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://sldn.softlayer.com/reference/services/SoftLayer_Network_SecurityGroup){: new_window}
* [*SoftLayer_Virtual_Guest_Network_Component* API ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest_Network_Component){: new_window}

You can also use the SoftLayer API Python Client to interact with security groups. For more information, see the following links:
* [SoftLayer API Python Client: Working with Virtual Servers ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://softlayer-python.readthedocs.io/en/latest/cli/vs.html){: new_window}
* [Python examples for softlayer_network_securitygroup ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://softlayer.github.io/classes/softlayer_network_securitygroup/){: new_window}