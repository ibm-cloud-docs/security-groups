---



copyright:
  years: 2017, 2018
lastupdated: "2019-11-14"

keywords: assign, instance, security group

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank_"}
{:pre: .pre}
{:note: .note}
{:important: .important}
{:tip: .tip}
{:table: .aria-labeledby="caption"}
{:external: target="_blank_" .external}

# Assigning Instances to the Security Group
{: #assigning-instances-to-the-security-group}

You can assign IBM™ Cloud Security Group objects to instances in one of two ways.
{: shortdesc}

## Using the Security Menu
{: #using-the-security-menu}

1. From the [IBM Cloud console](https://cloud.ibm.com/) dashboard, click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to get to the Classic Infrastructure landing page.
2. From the Classic Infrastructure menu, select **Security** >  **Network Security** > **Security Groups** to get to the Security Groups page.
3. On the Security Groups page, click on the ![More icon](./images/more_icon.jpg) icon of the Security Group object you wish to assign instances to, then select **Manage Instances**.
4. Select the instance and interface to apply to the Security Group.

	![Security Menu Instance](./images/security_assign.jpg)

	In the figure, the "allow_icmp" Security Group (created in the [first step](/docs/infrastructure/security-groups?topic=security-groups-creating-a-security-group)) is applied to the private interface (`10.0.2.219`) of "jpmongevsi4".

	Note how the **Attached Instances** count increased from `0` to `1`.

5. Click **Save** to apply the changes.

6. Reboot your instance.

	This is a one-time-only step per network interface for instances not created with a security group.
  {: note}

## Using the Devices Menu
{: #using-the-devices-menu}

1. From the [IBM Cloud console](https://cloud.ibm.com/) dashboard, click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to get to the Classic Infrastructure landing page.
2. From the Classic Infrastructure menu, select **Devices** >  **Device List** to get to the Devices page.
3. On the Devices page, click the instance name where you want to apply the Security Group object.
4. Select **Modify** and mark the Security Group object you want to associate with the instance.

	![Device Menu Instance](./images/device_assign.jpg)

	This figure shows the "allow_icmp" Security Group object being assigned to the private interface of jpmongevsi4 instance.
5. Click **Save** to apply the changes.

6. Reboot the instance.

	This is a one-time-only step per network interface for instances not created with a security group.
  {: note}

## Next step...
{: #next-step-1}

[Edit the Security Group](/docs/infrastructure/security-groups?topic=security-groups-editing-a-security-group) to modify its parameters.  
