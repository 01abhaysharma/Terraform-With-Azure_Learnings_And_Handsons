# Data source block

Data source blocks are used for referncing the alrady created resource.

In the "Terraform Resource Block" example "myresourcegroup" has already been created previously or within another Terraform deployment, utilising the Data source - you can make reference to the resource group.

## Data source block example

The below example references the data resource `azurerm_resource_group` `rg` to deploy Azure Storage Account `mystorageaccount.
- reference of `resource_group_name` & `location` is using the data reference of Resource Group.

```terraform
data "azurerm_resource_group" "rg" {
  name = "myresourcegroup"
  location = "East US"
}

resource "azurerm_storage_account" "sa" {
  name                     = "mystorageaccount"
  resource_group_name      = data.azurerm_resource_group.rg.name
  location                 = data.azurerm_resource_group.rg.location
  account_tier             = "Standard"
  account_replication_type = "LRS"
}
}
```
