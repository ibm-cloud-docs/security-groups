---

copyright:
  years: 2017, 2020
lastupdated: "2020-08-10"

keywords: manage, details, edit, configure

subcollection: security-groups

---

{{site.data.keyword.attribute-definition-list}}

# Managing security groups
{: #managing-sg}

You can manage security groups by using the Security Groups page, or the Device Details page in the {{site.data.keyword.cloud}} console.
{: shortdesc}

## Managing security groups from the Security Groups page
{: #managing-security-groups-from-security-groups-page}

To manage security groups from the Security Groups page, complete the following steps:

1. From the [IBM Cloud console](https://cloud.ibm.com/), click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to view the Classic Infrastructure landing page.
2. From the Classic Infrastructure menu, select **Security** >  **Network Security** > **Security Groups** to view the Security Groups page.
3. On the Security Groups page, you can complete several management tasks.
     * View a list of security groups.
     * Create a group.
     * Edit group information.
     * Duplicate a group.
     * Delete a group.

## Managing security group rules from the Security Groups page
{: #managing-security-group-rules-from-security-groups-page}

To manage security group rules from the Security Groups page, complete the following steps:

1. From the [IBM Cloud console](https://cloud.ibm.com/), click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to get to the Classic Infrastructure landing page.
2. From the Classic Infrastructure menu, select **Security** >  **Network Security** > **Security Groups** to get to the Security Groups page.
3. On the Security Groups page, click on a security group name to open the Details page.
4. On the Security Group Details page, you can complete several management tasks.
     * View a list of rules that are defined for the security group.
     * Create new rules.
     * Edit a rule.
     * Delete a rule.
     * View the virtual server instances and the associated interfaces that are assigned to the security group.

If you delete the last rule in a security group, then inbound and outbound traffic is not allowed by this security group.
{: tip}

## Managing security groups from the Device Details page
{: #managing-security-groups-from-device-details-page}

To manage security groups from the Device Details page, complete the following steps:

1. From the [IBM Cloud console](https://cloud.ibm.com/), click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to get to the Classic Infrastructure landing page.
2. From the Classic Infrastructure menu, select **Devices** > **Device List** to get to the Devices page.
3. On the Devices page, select the device name of the virtual server that you ordered to view its details.
4. In the Security Group section, you can assign predefined security groups to a network interface of a virtual server instance.
     
   The first time that you assign an existing security group to a network interface (public or private), a restart is required for each interface.  However, if the public and private interfaces were assigned to the security group at the same time, then only one restart is required. After a restart, changes are automatically applied.
   {: important}

     When you assign a new security group, it prevents new connections from being established according to the security group rule definitions. However, existing socket connections are not terminated.

     If you remove the last security group that is assigned to a virtual server instance, then the virtual server traffic is no longer limited by security groups. A security group firewall no longer exists.
     {: tip}

5. After you finish making changes, click **Save**.
