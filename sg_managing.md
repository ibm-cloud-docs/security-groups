---



copyright:
  years: 2017, 2019
lastupdated: "2019-06-11"

keywords: manage, details, edit, configure

subcollection: security-group

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank_"}
{:note: .note}
{:important: .important}
{:tip: .tip}
{:external: target="_blank_" .external}

# Managing Security Groups
{: #managing-sg}

You can manage security groups by using the Security Groups page or the Device Details page in the {{site.data.keyword.cloud}} console.
{: shortdesc}

## Managing security groups from Security Groups page
{: #managing-security-groups-from-security-groups-page}

To manage security groups from the Security Groups page, complete the following steps:

1. From the [IBM Cloud console](https://cloud.ibm.com/) dashboard, click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to get to the Classic Infrastructure landing page.
2. From the Classic Infrastructure menu, select **Security** >  **Network Security** > **Security Groups** to get to the Security Groups page.
3. On the Security Groups page, you can complete several management tasks.
     * View a list of security groups.
     * Create a group.
     * Edit group information.
     * Duplicate a group.
     * Delete a group.

## Managing security group rules from Security Groups page
{: #managing-security-group-rules-from-security-groups-page}

To manage security group rules from the Security Groups page, complete the following steps:

1. From the [IBM Cloud console](https://cloud.ibm.com/) dashboard, click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to get to the Classic Infrastructure landing page.
2. From the Classic Infrastructure menu, select **Security** >  **Network Security** > **Security Groups** to get to the Security Groups page.
3. On the Security Groups page, click on a security group name to open the Details page.
4. On the Security Group Details page, you can complete several management tasks.
     * View a list of rules that are defined for the security group.
     * Create new rules.
     * Edit a rule.
     * Delete a rule.
     * View the virtual server instances and the associated interfaces that are assigned to the security group.

If you delete the last rule in a security group, then no inbound or outbound traffic is allowed by this security group.
{: tip}

## Managing security groups from Device Details page
{: #managing-security-groups-from-device-details-page}

To manage security groups from the Device Details page, complete the following steps:

1. From the [IBM Cloud console](https://cloud.ibm.com/) dashboard, click the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) > **Classic Infrastructure** to get to the Classic Infrastructure landing page.
2. From the Classic Infrastructure menu, select **Devices** >  **Device List** to get to the Devices page.
3. On the Devices page, select the device name of the virtual server you ordered to get to the Devices Details page.
4. On the Device Details page, verify that you are on the **Configuration** tab.
5. Under the Security Group section, you can complete several management tasks.
     * View the security groups and rules.
     * Assign security groups to a network interface of a virtual server instance.
     * Remove security groups from a network interface of a virtual server instance.

     The first time that you assign an existing security group to a network interface (public or private), a restart is required for each interface.  However, if the public and private interfaces were assigned to the security group at the same time, then only one restart is required.  After a restart, changes are automatically applied.
     {: important}

     When you assign a new security group, it prevents new connections from being established according to the security group rule definitions. However, existing socket connections are not terminated.

     If you remove the last security group that is assigned to a virtual server instance, then the virtual server traffic is no longer limited by security groups. A security group firewall no longer exists.
     {: tip}

6. When you finish making changes, click **Save**.
