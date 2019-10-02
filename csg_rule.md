---



copyright:
  years: 2017
lastupdated: "2018-11-10"

keywords: create, new, rule, ssh, icmp

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:note: .note}
{:important: .important}
{:tip: .tip}
{:external: target="_blank" .external}

# Creating a New Rule
{: #creating-a-new-rule}

Allow incoming requests (SSH & ICMP) and their related (outgoing) traffic flows by performing the following procedure:

1. From the [IBM Cloud console](https://cloud.ibm.com/) dashboard, click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to get to the Classic Infrastructure landing page.
2. From the Classic Infrastructure menu, select **Security** >  **Network Security** > **Security Groups** to get to the Security Groups page.
3. On the Security Groups page, select the Security Group object to which you want to add a rule.
4. On the Rules tab, click the **Create Rule +** button.
5. Specify the rule's Direction, IP Type, Protocol, Port Range, Type, Code and Source when applicable (based on the Protocol selection).

	Unless you are using another Security Group as the source, leave **Source Type** as "CIDR Block".

	![Create a rule](./images/rule_sg.jpg)

	The figure shows **All ICMP** selected as the protocol, which means all ICMP Types and Codes will be allowed. Additionally, the Source field is being left empty, using the default value of `0.0.0.0/0` -- the equivalent to any IP address or subnet.

6. Click **OK** to finish.

## Next step...
{: #next-step-3}

[Assign instances to the Security Group](/docs/infrastructure/security-groups?topic=security-groups-assigning-instances-to-the-security-group) using either the Security Menu or the Device Menu.
