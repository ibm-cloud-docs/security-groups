---



copyright:
  years: 2017
lastupdated: "2017-08-08"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Getting started with Security Groups

You can use Security Groups to enact a set of IP filter rules that define how to handle incoming and outgoing traffic to both the public and private interfaces of a virtual server instance.
{:shortdesc}

## Pain Points and Solutions
There are a few difficult network security scenarios you might encounter that can be alleviated by using Seurity Groups.

### Security from the start
**Pain point:** Customers want to secure their virtual server as soon as it is provisioned. They want complete control over the traffic passing through the server from the point when it was provisioned.

**Solution:** Use Security Groups at the time of ordering the virtual server. It is protected right from the time it is provisioned for the customer.

### Cost-efficient instance level firewall
**Pain point:** Customers want to have granular control over traffic at an instance level (apart from network-level firewalling), but at the same time, the costs of a shared hardware firewall (which is IBM’s other instance level multi-tenant firewall offering) can add up quickly if the customer desired to protect multiple servers in different data centers.

**Solution:** There is no extra charge for using the Security Groups feature. Use Security Groups for all virtual servers that need protection in any of our global data centers.

### Globally scalable and easily manageable firewall
**Pain point:** Customers want to avoid configuring firewall rules on each server separately. Instead, they want an easily manageable firewall solution which spans servers in different global data centers.

**Solution:** Define N Security Groups for N different types of servers in your cloud workload. Manage all rules for a security group in one place. Manage the security group associations appropriately with the virtual servers.