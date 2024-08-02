---

copyright:
  years: 2024
lastupdated: "2024-08-02"

keywords: create, new, rule, ssh, icmp

subcollection: security-groups

---

{{site.data.keyword.attribute-definition-list}}

# Creating a rule
{: #creating-a-new-rule}

You can allow incoming requests (SSH & ICMP) and their related (outgoing) traffic flows for your {{site.data.keyword.cloud}} security groups by performing the instructions here.
{: shortdesc}

1. From the [IBM Cloud console](https://cloud.ibm.com/), click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to get to the Classic Infrastructure landing page.
1. From the Classic Infrastructure menu, select **Security** >  **Network Security** > **Security Groups** to get to the Security Groups page.
1. On the Security Groups page, select the security group object to which you want to add a rule.
1. On the Rules tab, click the **Create rule +** button.
1. Specify the rule's Direction, IP Type, Protocol, Port Range, Type, Code and Source when applicable (based on the Protocol selection).

   Unless you are using another Security Group as the source, leave **Source Type** as **CIDR Block**.

   The figure shows **All ICMP** selected as the protocol, which means all ICMP types and codes are allowed. Additionally, the Source field is being left empty, using the default value of `0.0.0.0/0` -- the equivalent to any IP address or subnet.

1. Click **OK** to finish.

## Next step...
{: #next-step-3}

[Assign instances to the security group](/docs/security-groups?topic=security-groups-assigning-instances-to-the-security-group) using either the Security menu or the Device menu.
