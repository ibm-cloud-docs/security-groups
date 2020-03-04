---

copyright:
  years: 2017
lastupdated: "2019-11-14"

keywords: create, rules, assign, interface, virtual server

subcollection: security-group
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank_"}
{:note: .note}
{:important: .important}
{:tip: .tip}


# Creating security groups and rules
{: #creating-security-groups}

You can create an IBM™ Cloud Security Group and its associated rules and then assign it to the interfaces of one or more virtual server instances to enable a virtual firewall.
{: shortdesc}

## Creating a security group
{: #creating-a-security-group-1}

To create a security group, complete the following steps:

1. From the [IBM Cloud console](https://cloud.ibm.com/) dashboard, click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to get to the Classic Infrastructure landing page.
2. From the Classic Infrastructure menu, select **Security** >  **Network Security** > **Security Groups** to get to the Security Groups page.
3. On the Security Groups page, click the **Create Group +** button.
4. Enter a name and description for the security group and click **Create Group**.

**Create group with a default rule to allow all outbound traffic** is selected by default. You can clear this field to create the security group with no rules. A security group with no rules blocks all traffic (both inbound and outbound).
{: note}

## Creating security group rules
{: #creating-security-group-rules}

To create a security group rule, complete the following steps:

1. From the [IBM Cloud console](https://cloud.ibm.com/) dashboard, click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to get to the Classic Infrastructure landing page.
2. From the Classic Infrastructure menu, select **Security** >  **Network Security** > **Security Groups** to get to the Security Groups page.
3. On the Security Groups page, click a security group name to open the Details page and click the **Create Rule +** button.
4. On the Create Rule page, enter all appropriate attributes (such as direction, IP type, protocol, and source/destination information). When finished, click **Ok**.

Selecting the optional source or destination fields will restrict the new rule so it only applies to traffic to/from the specified source/destination. Source and destination fields can specify either a Classless Inter-Domain Routing (CIDR) block or a security group.
{: note}

A CIDR block facilitates routing of a block of IP addresses.  If you select CIDR as the type, then you must specify an IP address range.

If you select security groups as the type, then you must select from a list of existing security groups. This selection allows any IP address from a device that is attached to the selected security group. If a virtual server is configured to have multiple IP addresses, only the primary IPv4 and IPv6 addresses are used by these remote security group rules.
