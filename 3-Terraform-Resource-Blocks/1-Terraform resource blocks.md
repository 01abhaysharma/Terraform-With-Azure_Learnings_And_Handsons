# Terraform Resource Blocks

They are the most commonly used component within Terraform. They are used for deploying one or more resources. 

Each resource block will deploy or destroy at least one Azure resource. 

Resource blocks include virtual machines, virtual networks, resource groups etc.

## Resource block example

The below contains a resource called `rg`,

that uses the terraform resource `azurerm_resource_group`,

to create an Azure Resource Group called `myresourcegroup` in region `East US`

```terraform
resource "azurerm_resource_group" "rg" {
  name     = "myresourcegroup"
  location = "East US"
}
```
