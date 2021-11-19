---

copyright:
  years: 2021
lastupdated: "2021-08-12"

subcollection: security-groups

---

{{site.data.keyword.attribute-definition-list}}

# Setting up Terraform for security groups
{: #terraform-setup-sgs}

Terraform on {{site.data.keyword.cloud}} enables predictable and consistent provisioning of {{site.data.keyword.cloud_notm}} services so that you can rapidly build complex, multi-tier cloud environments following Infrastructure as Code (IaC) principles. Similar to using the {{site.data.keyword.cloud_notm}} CLI or API and SDKs, you can automate the provisioning, update, and deletion of your security group instances by using HashiCorp Configuration Language (HCL).
{: shortdesc}

Looking for a managed Terraform on {{site.data.keyword.cloud}} solution? Try out [{{site.data.keyword.bplong}}](/docs/schematics?topic=schematics-getting-started). With {{site.data.keyword.bpshort}}, you can use the Terraform scripting language that you are familiar with, but you don't have to worry about setting up and maintaining the Terraform command line and the {{site.data.keyword.cloud}} Provider plug-in. {{site.data.keyword.bpshort}} also provides pre-defined Terraform templates that you can easily install from the {{site.data.keyword.cloud}} catalog.
{: tip}

## Installing Terraform and configuring resources for security groups
{: #install-terraform-sgs}

To install Terraform and configure resources for security groups:

1. Follow the [Terraform on {{site.data.keyword.cloud}} getting started tutorial](/docs/ibm-cloud-provider-for-terraform?topic=ibm-cloud-provider-for-terraform-getting-started) to install the Terraform CLI and configure the {{site.data.keyword.cloud}} Provider plug-in for Terraform. The plug-in abstracts the {{site.data.keyword.cloud}} APIs that are used to provision, update, or delete security group service instances and resources.
2. Create a Terraform configuration file that is named `main.tf`. In this file, you add the configuration to create a security group service instance. For more information, see the [Terraform documentation](https://www.terraform.io/docs/language/index.html){: external}.

   The security group resource in the following example is named `sg1`. For more information, see the [ibm_security_group](https://registry.terraform.io/providers/IBM-Cloud/ibm/latest/docs/resources/security_group){: external} usage example.

   ```terraform
   resource "ibm_security_group" "sg1" {
       name = "sg1"
       description = "allow my app traffic"
   }
   ```
   {: codeblock}

3. Initialize the Terraform CLI.

   ```sh
   terraform init
   ```
   {: codeblock}

4. Create a Terraform execution plan. The Terraform execution plan summarizes all the actions that need to be run to create the security group instance in your account.

   ```sh
   terraform plan
   ```
   {: codeblock}

5. Create the security group instance in {{site.data.keyword.cloud_notm}}.

   ```sh
   terraform apply
   ```
   {: codeblock}

6. From the [{{site.data.keyword.cloud_notm}} resource list](/resources){: external}, select the security group instance that you created and note the instance ID.
