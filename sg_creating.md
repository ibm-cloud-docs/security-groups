---



copyright:
  years: 2017
lastupdated: "2017-04-27"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}


# Creating security groups and rules
{: #creating-security-groups}

You can create a security group and its associated rules and then assign it to the interfaces of one or more virtual server instances to enable a virtual firewall.
{:shortdesc}

## Creating a security group

To create a security group, complete the following steps:
{:shortdesc}
 
1. In the [Customer Portal ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/) navigation, select **Security -> Network Security -> Security Groups**.
2. On the Security Groups page, click **Create Group**.
3. Enter a name and description for the security group and click **Create Group** again.

**Note:** "Create group with a default rule to allow all outbound traffic." is selected by default. You can clear this field to create the security group with no rules. A security group with no rules blocks all traffic (both inbound and outbound).

## Creating security group rules

To create a security group rule, complete the following steps:
{:shortdesc}

1. In the [Customer Portal ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/) navigation, select **Security -> Network Security -> Security Groups**.
2. On the Security Groups page, click a security group name to open the Details page and select **Create Rule**.
3. On the Create Rule page, enter all appropriate attributes (such as direction, IP type, protocol, and source/destination information). When finished, click **Ok**.

**Note**: Selecting the optional source or destination fields will restrict the new rule so it only applies to traffic to/from the specified source/destination.  Source and destination fields can specify either a Classless Inter-Domain Routing (CIDR) block or a security group. 

A CIDR block facilitates routing of a block of IP addresses.  If you select CIDR as the type, then you must specify an IP address range. 

If you select security groups as the type, then you must select from a list of existing security groups. This selection allows any IP address from a device that is attached to the selected security group. If a virtual server is configured to have multiple IP addresses, only the primary IPv4 and IPv6 addresses are used by these remote security group rules.
