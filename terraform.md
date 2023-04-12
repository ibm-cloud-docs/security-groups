---

copyright:
  years: 2021, 2023
lastupdated: "2023-04-12"

subcollection: _your-subcollection_

---

{{site.data.keyword.attribute-definition-list}}

# Setting up Terraform for security groups
{: #terraform-setup}

Terraform on {{site.data.keyword.cloud}} enables predictable and consistent provisioning of {{site.data.keyword.cloud_notm}} services so that you can rapidly build complex, multi-tier cloud environments following Infrastructure as Code (IaC) principles. Similar to using the {{site.data.keyword.cloud_notm}} CLI or API and SDKs, you can automate the provisioning, update, and deletion of your security group instances by using HashiCorp Configuration Language (HCL).
{: shortdesc}

Looking for a managed Terraform on {{site.data.keyword.cloud}} solution? Try out [{{site.data.keyword.bplong}}](/docs/schematics?topic=schematics-getting-started). With {{site.data.keyword.bpshort}}, you can use the Terraform scripting language that you are familiar with, but you don't have to worry about setting up and maintaining the Terraform command line and the {{site.data.keyword.cloud}} Provider plug-in. {{site.data.keyword.bpshort}} also provides pre-defined Terraform templates that you can easily install from the {{site.data.keyword.cloud}} catalog.
{: tip}

## Installing Terraform and configuring resources for _service-name_
{: #install-terraform}

Before you can create an authorization by using Terraform, make sure that you have completed the following:

* Make sure that you have the required access to create and work with security group resources.
* Install the Terraform CLI and configure the {{site.data.keyword.cloud_notm}} Provider plug-in for Terraform. For more information, see the tutorial for [Getting started with Terraform on {{site.data.keyword.cloud}}](/docs/ibm-cloud-provider-for-terraform?topic=ibm-cloud-provider-for-terraform-getting-started). The plug-in abstracts the {{site.data.keyword.cloud_notm}} APIs that are used to complete this task.
* Create a Terraform configuration file that is named `main.tf`. In this file, you define resources by using HashiCorp Configuration Language. For more information, see the [Terraform documentation](https://www.terraform.io/docs/language/index.html){: external}.

1. Create a security groups instance by using the `ibm_resource_instance` resource argument in your `main.tf` file.

   The security group resource in the following example is named `sg1`. For more information, see the [ibm_security_group](https://registry.terraform.io/providers/IBM-Cloud/ibm/latest/docs/resources/security_group){: external} usage example.

   ```terraform
   resource "ibm_security_group" "sg1" {
       name = "sg1"
       description = "allow my app traffic"
   }
   ```
   {: codeblock}

2. After you finish building your configuration file, initialize the Terraform CLI. For more information, see [Initializing Working Directories](https://www.terraform.io/cli/init){: external}.

   ```sh
   terraform init
   ```
   {: codeblock}

3. Provision the resources from the `main.tf` file. For more information, see [Provisioning Infrastructure with Terraform](https://www.terraform.io/cli/run){: external}.

   1. Run `terraform plan` to generate a Terraform execution plan to preview the proposed actions.

      ```terraform
      terraform plan
      ```
      {: pre}

   1. Run `terraform apply` to create the resources that are defined in the plan.

      ```terraform
      terraform apply
      ```
      {: pre}

6. From the [{{site.data.keyword.cloud_notm}} resource list](/resources){: external}, select the {{site.data.keyword.keymanagementserviceshort}} instance that you created and note the instance ID.
7. Verify that the access policy is successfully assigned. For more information, see [Reviewing assigned access in the console](/docs/account?topic=account-assign-access-resources#review-your-access-console).
