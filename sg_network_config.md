---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: configuration, network, virtual server, instance, security

subcollection: security-groups


---

{{site.data.keyword.attribute-definition-list}}

# Existing network configurations and security groups
{: #existing-network-configurations-and-security-groups}

A security group augments any existing network configuration. Therefore, a security group cannot span across networks that cannot communicate with one another.
{: shortdesc}

If virtual server instances cannot communicate with one another, adding them to a security group does not change that behavior. Gateways must allow the traffic that is defined by the selected security groups.

If your account is enabled for custom private addressing (CPA) as well as security groups, be aware that security groups are scoped to the account level, not the network level. Security groups are defined by IP addresses, not private networks.

Security groups are available in all data centers with virtual server instance provisioning.
