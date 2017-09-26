---



copyright:
  years: 2017
lastupdated: "2017-08-10"


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Managing security groups
{: #managing-sg}

You can manage security groups by using the Security Groups page or the Device Details page in the Customer portal.
{:shortdesc}

## Managing security groups from Security Groups page

To manage security groups from the Security Groups page, complete the following steps:
{:shortdesc}

1. From the [Customer Portal ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/) navigation, select **Security -> Network Security -> Security Groups**.
2. Under the Security Group section, you can complete several management tasks.
     * View a list of security groups.
     * Create a group.
     * Edit group information.
     * Duplicate a group.
     * Delete a group.
     
## Managing security group rules from Security Groups page

To manage security group rules from the Security Groups page, complete the following steps:
{:shortdesc}

1. From the [Customer Portal ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/) navigation, select **Security -> Network Security -> Security Groups**.
2. Click a security group name to open the Details page.
3. From the Security Group Details page, you can complete several management tasks.
     * View a list of rules that are defined for the security group.
     * Create new rules.
     * Edit a rule.
     * Delete a rule.
     * View the virtual server instances and the associated interfaces that are assigned to the security group.
     
**Tip:** If you delete the last rule in a security group, then no inbound or outbound traffic is allowed by this security group.
     
## Managing security groups from Device Details page

To manage security groups from the Device Details page, complete the following steps:
{:shortdesc}

1. From the [Customer Portal ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/), select **Devices -> Device List**.
2. Select the device name of the virtual server you ordered. The Device Details page opens.
3. From the Device Details page, verify that you are on the **Configuration** tab.
4. Under the Security Group section, you can complete several management tasks.
     * View the security groups and rules.
     * Assign security groups to a network interface of a virtual server instance.
     * Remove security groups from a network interface of a virtual server instance.
     
     **Important** : The first time that you assign an existing security group to a network interface (public or private), a restart is required for each interface.  However, if the public and private interfaces were assigned to the security group at the same time, then only one restart is required.  After a restart, changes are automatically applied.
     
     When you assign a new security group, it prevents new connections from being established according to the security group rule definitions. However, existing socket connections are not terminated.

     **Tip**: If you remove the last security group that is assigned to a virtual server instance, then the virtual server traffic is no longer limited by security groups. A security group firewall no longer exists.
     
6. When you finish making changes, click **Save**.
