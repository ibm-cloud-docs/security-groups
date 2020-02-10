---



copyright:
  years: 2017, 2018
lastupdated: "2019-11-14"

keywords: add, order, group

subcollection: security-groups
---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank_"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:note: .note}
{:important: .important}
{:tip: .tip}
{:external: target="_blank_" .external}

# Adding a pre-defined Security Group during ordering
{: #adding-a-pre-defined-security-group-during-ordering}

This step-by-step procedure shows you how to add existing or pre-defined IBM™ Cloud Security Groups to instances during the ordering process.
{: shortdesc}

You can use Security Groups to enact a set of IP filter rules that define how to handle incoming and outgoing traffic to both the public and private interfaces of a virtual server instance.

![Custom Security Group](./images/goal2.jpg)

## What you'll need
{: #what-you-ll-need-2}

For this example the following objects and items will be used:

| Resource Name  | Operating System | Type | Location/DC | IP/Subnet |
|:------------- |:---------------:| -------------:| :---------------:| ---------------:|
| allow_ssh1 | Not Applicable  | Security Group | Not Applicable/Any | 0.0.0.0/0 |
|jpmongevsi2.testing.com | Ubuntu 16.04 | Virtual server instance | Dallas 10 Pod 01 | 10.0.0.21 |
|jpmongevsi4.testing.com | Ubuntu 16.04 | Virtual server instance |	Dallas 10 Pod 01	| 10.0.2.219 |

## Order a Security Group
{: #order-a-security-group}

To order a virtual server instance and assign a security group, perform the following procedure:

1. From your browser, open the [IBM Cloud Catalog](https://cloud.ibm.com/catalog) and log in to your account.

2. Select **Compute** on the left side of the page, then click on the **Virtual Server** tile to get to the Virtual Server page.

3. Configure your Virtual Server based on your requirements.
  
  For complete information on provisioning a VSI, refer to the [Virtual Server Instance documentation](/docs/vsi?topic=virtual-servers-getting-started-tutorial).

4. From the Network Interface section, use the menus to select any predefined private or public security groups for your VSI.

  Only predefined security groups will display in these menu lists. To define a new security group, refer to [Creating Security Groups and Rules](/docs/security-groups?topic=security-groups-creating-security-groups)

5. Mark the Cloud Service terms and the Third-Party Service Agreement check box.

6. Finally, click **Create**.
