---



copyright:
  years: 2017, 2020
lastupdated: "2020-08-10"

keywords: assign, instance

subcollection: security-groups

---

{{site.data.keyword.attribute-definition-list}}

# Assigning instances to the security group
{: #assigning-instances-to-the-security-group}

You can assign {{site.data.keyword.cloud}} security group objects to instances in one of two ways.
{: shortdesc}

## Using the Security menu
{: #using-the-security-menu}

1. From the [IBM Cloud console](https://cloud.ibm.com/), click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to view the Classic Infrastructure landing page.
1. From the Classic Infrastructure menu, select **Security** >  **Network Security** > **Security Groups** to view the Security Groups page.
1. On the Security Groups page, click the ![More icon](./images/more_icon.jpg) icon of the Security Group object that you want to assign instances to, then select **Manage Instances**.
1. Select the instance and interface to apply to the security group.
1. Click **Save** to apply the changes.
1. Restart your instance.

   This is a one-time-only step per network interface for instances not created with a security group.
   {: note}

## Using the Devices menu
{: #using-the-devices-menu}

1. From the [IBM Cloud console](https://cloud.ibm.com/), click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to view the Classic Infrastructure landing page.
1. From the Classic Infrastructure menu, select **Devices** > **Device List** to view the Devices page.
1. On the Devices page, click the instance name where you want to apply the security group object.
1. In the **Security Groups** column, click **View** and select the security group objects that you want to associate with the instance.
1. In the **Security group changes** modal that appears, click **OK** to apply the changes.
1. Restart the instance.

   This is a one-time-only step per network interface for instances not created with a security group.
   {: note}

## Next step
{: #next-step-1}

[Edit the security group](/docs/security-groups?topic=security-groups-editing-a-security-group) to modify its parameters.  
