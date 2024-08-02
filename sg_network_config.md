---

copyright:
  years: 2024
lastupdated: "2024-08-02"

keywords: configuration, network, virtual server, instance, security

subcollection: security-groups


---

{{site.data.keyword.attribute-definition-list}}

# Existing network configurations and security groups
{: #existing-network-configurations-and-security-groups}

A security group augments any existing network configuration. Therefore, a security group cannot span across networks that cannot communicate with one another.
{: shortdesc}

Security groups are interface constructs, they're not IP specific. When a virtual server has a public interface with a security group applied, the security group also applies to the interfaces assigned to the portable subnet.

To prevent DHCP spoofing, a `DROP` rule is added as a mandate whenever the security group is applied. As such, trying to set a DHCP server using a secondary portable subnet will not work with a security group applied.

If virtual server instances cannot communicate with one another, adding them to a security group does not change that behavior. Gateways must allow the traffic that is defined by the selected security groups.

If your account is enabled for custom private addressing (CPA) as well as security groups, be aware that security groups are scoped to the account level, not the network level. Security groups are defined by IP addresses, not private networks.

Security groups are available in all data centers with virtual server instance provisioning.
