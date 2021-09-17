---



copyright:
  years: 2017, 2018
lastupdated: "2021-09-14"

keywords: order, overview, use cases, security groups

subcollection: security-groups


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank_"}
{:note: .note}
{:important: .important}
{:tip: .tip
{:external: target="_blank_" .external}

# Getting started with IBM security groups
{: #getting-started}

You can use security groups to enact a set of IP filter rules that define how to handle incoming and outgoing traffic to both the public and private interfaces of a virtual server instance.
{: shortdesc}

To get started, order a virtual server instance and assign a security group.

1. From your browser, open the [IBM Cloud catalog](https://cloud.ibm.com/catalog) and log in to your account.

1. Select **Services** > **Compute**, then click the **Virtual Server for Classic** tile to show the Virtual server instance page.

1. Configure your virtual server based on your requirements. 

   For more information, see [Getting started with virtual servers](/docs/virtual-servers).

1. In the Network Interface section, use the menus to select any predefined private or public security groups for your virtual server instance.

   Only predefined security groups show in these menu lists. To define a new security group, see [Creating security groups and rules](/docs/security-groups?topic=security-groups-creating-security-groups).

1. Click **Create**.

## Use cases and solutions
{: #use-cases-and-solutions}

The following sections describe a few difficult network security scenarios that can be alleviated by using security groups.

### Security from the start
{: #security-from-the-start}

**Security scenario:** You want to secure your virtual server as soon as it is provisioned. You also want complete control over the traffic that passes through the server from the point when it was provisioned.

**Solution:** Use security groups when you order a virtual server. That way, your server is protected when it is first provisioned.

### Cost-efficient instance level firewall
{: #cost-efficient-instance-level-firewall}

**Security scenario:** Customers want granular control over traffic at an instance level (apart from network-level firewalls). However, at the same time, the costs of a shared hardware firewall can add up quickly if you need to protect multiple servers in different data centers.

**Solution:** You do not incur extra charges for using security groups. You can use security groups for all virtual servers that need protection in any of our global data centers.

### Globally scalable and easily manageable firewall
**Security scenario:** You want to avoid configuring firewall rules on each server separately. Instead, you want an easily manageable firewall solution that spans servers in different global data centers.

**Solution:** Define `N` security groups for `N` different types of servers in your cloud workload. Manage all rules for a security group in one place. Manage the security group associations with the virtual servers.
