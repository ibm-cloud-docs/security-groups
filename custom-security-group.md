---

copyright:
  years: 2017, 2025
lastupdated: "2025-03-14"

keywords: create, manage, custom, instance, assign, edit

subcollection: security-groups

---

{{site.data.keyword.attribute-definition-list}}

# Creating and managing a custom security group
{: #creating-and-managing-a-custom-security-group}

In this tutorial learn how to create, assign instances to, and edit a custom {{site.data.keyword.cloud}} security group.
{: shortdesc}

## What you'll need
{: #what-you-ll-need-3}

For this example, the following objects and items are used:

| Resource Name  | Operating System | Type | Location/DC | IP/Subnet |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| Not Applicable/Any | 10.0.0.0/16 |
| allow_icmp | Not Applicable  | Security Group | Not Applicable/Any | 0.0.0.0/0 |
| allow_ssh | Not Applicable | Security Group | Not Applicable/Any | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Virtual server instance | Dallas 10 Pod 01 | 10.0.0.21 |
|jpmongevsi4.testing.com | Ubuntu 16.04 | Virtual server instance |	Dallas 10 Pod 01	| 10.0.2.219 |
{: caption="What you'll need" caption-side="bottom"}

Note that this tutorial makes use of a CPA private network/account, however, for practical purposes security groups behave the same way in both CPA accounts and regular accounts. Subnets 10.0.0.0/24 and 10.0.2.0/24 belong to the same CPA private network, which would be the equivalent of having a regular account with two or more virtual server instances connected to the same private subnet/VLAN.


## What you'll accomplish
{: #what-you-ll-accomplish-3}

In this tutorial, learn how to...

Task  | Description
------------- | -------------
[Create a security group](/docs/security-groups?topic=security-groups-creating-a-security-group) | Create and configure a custom security group, as opposed to using one predefined by the {{site.data.keyword.cloud_notm}} platform.
[Create a rule](/docs/security-groups?topic=security-groups-creating-a-new-rule) | Create a rule to allow incoming requests (SSH & ICMP) and their related (outgoing) traffic flows.
[Assign instances to the security group](/docs/security-groups?topic=security-groups-assigning-instances-to-the-security-group) | Assign security group objects to instances using either the Security menu or the Device menu.
[Edit a security group and its rules](/docs/security-groups?topic=security-groups-editing-a-security-group) | Modify the parameters of the security object and its rules.
{: caption="What you'll accomplish" caption-side="top"}
