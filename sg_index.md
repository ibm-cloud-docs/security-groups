---



copyright:
  years: 2017, 2018
lastupdated: "2018-11-10"

keywords: order, begin, overview, use cases, solutions

subcollection: security-group


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:note: .note}
{:important: .important}
{:tip: .tip}

# Getting Started with Security Groups
{: #getting-started}

You can use Security Groups to enact a set of IP filter rules that define how to handle incoming and outgoing traffic to both the public and private interfaces of a virtual server instance.
{: shortdesc}

To get started, order a virtual server instance (VSI) and assign a security group.

1. From your browser, open [Customer Portal ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/) and log in to your account.
2. Locate the **Order** section and click **Devices**.
3. On the Devices page, click **Hourly** or **Monthly** for one of the Virtual Server offerings.
4. On the **Configure your Cloud Server** order page, you must select a data center that supports security groups.
5. Complete any other necessary information and click **Add to Order**. The Checkout page opens.
6. Complete the **Configure Security Groups** information.
7. You can select any of the predefined security groups to apply to the private or public interfaces on the virtual server.
8. Finally, click **Submit Order**.

## Use Cases and Solutions
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
