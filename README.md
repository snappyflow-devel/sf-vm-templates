# SnappyFlow Templates for provisioning applications in private and public cloud
This repository consists of templates for provisioning application. These templates are meant to be used from SnappyFlow. These templates are based on Terraform or AWS Cloudformation. Developers can use these templates directly from cloudformation or Terraform.

## Terrafrom reference
The recommended framework is tereraform. Please go throguh below links to familiarize yourself with terrafrom constructs.
 - [https://learn.hashicorp.com/terraform/](https://learn.hashicorp.com/terraform/)
 - [Terrafrom Interpolation Syntax](https://www.terraform.io/docs/configuration/interpolation.html)

## Guidelines for creating a new template.
 - Every template should be committed to a new directory.
 - Top level of template directory should have a file [template_info.json](template_info.md) and [parameters.json](parameters.md).
 - Refer [Creating-a-new-template.md](Creating-a-new-template.md).
 - Once template development is complete, it can be promoted to production by adding to **templates_list_production.json** file.
 - Template which are not listed in templates_list_production.json file are not availabe on SnappyFlow servers marked as production servers.
 - _If you are creating AWS cloudformation based template, then template folder contains only template_info.json and actual cloudformation template_ 
 - __[integration with SnappyFlow](Integration-With-SnappyFlow.md)__
