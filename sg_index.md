---



copyright:
  years: 2017, 2018
lastupdated: "2019-11-14"

keywords: order, begin, overview, use cases, solutions

subcollection: security-group


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank_"}
{:note: .note}
{:important: .important}
{:tip: .tip
{:external: target="_blank_" .external}

# Getting started with IBM Security Groups
{: #getting-started}

You can use Security Groups to enact a set of IP filter rules that define how to handle incoming and outgoing traffic to both the public and private interfaces of a virtual server instance.
{: shortdesc}

To get started, order a Virtual Server Instance (VSI) and assign a security group.

1. From your browser, open the [IBM Cloud Catalog](https://cloud.ibm.com/catalog) and log in to your account.

2. Select **Compute** on the left side of the page, then click on the **Virtual Server** tile to get to the Virtual Server page.

3. Configure your Virtual Server based on your requirements.

  For complete information on provisioning a VSI, refer to the [Virtual Server Instance documentation](/docs/vsi?topic=virtual-servers-getting-started-tutorial).

4. From the Network Interface section, use the menus to select any predefined private or public security groups for your VSI.

  Only predefined security groups will display in these menu lists. To define a new security group, refer to [Creating Security Groups and Rules](/docs/security-groups?topic=security-groups-creating-security-groups)

5. Mark the Cloud Service terms and the Third-Party Service Agreement check box.

6. Finally, click **Create**.

## Use cases and solutions
{: #use-cases-and-solutions}

The sections below describe a few difficult network security scenarios you might encounter that can be alleviated by using Security Groups.

### Security from the start
{: #security-from-the-start}

**Security scenario:** Customers want to secure their virtual server as soon as it is provisioned. They want complete control over the traffic passing through the server from the point when it was provisioned.

**Solution:** Use Security Groups at the time of ordering the virtual server. That way, your server is protected right from the time it is provisioned.

### Cost-efficient instance level firewall
{: #cost-efficient-instance-level-firewall}

**Security scenario:** Customers want to have granular control over traffic at an instance level (apart from network-level firewalls), but at the same time, the costs of a shared hardware firewall (which is another instance level by IBM© of a multi-tenant firewall offering) can add up quickly if the customer needs to protect multiple servers in different data centers.

**Solution:** There is no extra charge for using the Security Groups feature. Use Security Groups for all virtual servers that need protection in any of our global data centers.

### Globally scalable and easily manageable firewall
**Security scenario:** Customers want to avoid configuring firewall rules on each server separately. Instead, they want an easily manageable firewall solution that spans servers in different global data centers.

**Solution:** Define `N` Security Groups for `N` different types of servers in your cloud workload. Manage all rules for a security group in one place. Manage the security group associations appropriately with the virtual servers.
