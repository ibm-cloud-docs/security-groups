---

copyright:
  years: 2017, 2019
lastupdated: "2019-11-14"

keywords: api, reference, slapi

subcollection: security-groups

---

{{site.data.keyword.attribute-definition-list}}

# Security group API reference
{: #api-reference}

The SoftLayer Application Programming Interface (API) is the development interface that gives developers and system administrators direct
interaction with SoftLayer's back-end system.
{: shortdesc}

The SoftLayer API (SLAPI) powers many of the features in the Customer Portal, which
typically means if an interaction is possible in the Customer Portal, it can also be run in the API. Because you can programmatically interact
with all portions of the SoftLayer environment within the API, you can use the API to automate tasks. For example, you can use the
SoftLayer_Virtual_Guest/createObject API to deploy a virtual server instance with a security group enabled.

The SoftLayer API is a Remote Procedure Call system. Each call involves sending data towards an API endpoint and receiving structured data
in return. The format used to send and receive data with the SLAPI depends on which implementation of the API you choose.

For more information about the SoftLayer API, virtual server, and security group APIs, see the following resources in the SoftLayer
Development Network:
* [SoftLayer API Overview](https://softlayer.github.io/reference/softlayerapi/){: external}
* [Getting Started with the SoftLayer API](http://sldn.softlayer.com/article/getting-started){: external}
* [SoftLayer_Virtual_Guest/createObject API](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest/createObject){: external}
* [SoftLayer_Network_SecurityGroup API](https://sldn.softlayer.com/reference/services/SoftLayer_Network_SecurityGroup){: external}
* [SoftLayer_Virtual_Guest_Network_Component API](http://sldn.softlayer.com/reference/services/SoftLayer_Virtual_Guest_Network_Component){: external}
