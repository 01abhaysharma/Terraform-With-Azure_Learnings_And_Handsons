## What is a Terraform Provider?

Terraform providers are plugins that allow Terraform to interact with the underlying API's of various services.

## Why do we need a Terraform Provider?

Providers are needed to allow Terraform to interact with the underlying API's of various services.

## What is a Terraform Azure Provider?

Terraform Azure provider is plugin that allow Terraform to interact with the underlying API's of Azure.

The Azure Provider is used to interact with the many resources supported by Azure Resource Manager (ARM).

## Azure Provider Configuration

The Azure Provider is used to configure the proper credentials before it can be used.

The Azure Provider can be configured using the Azure CLI. You can install Azure CLI using "Chocolaty". 

Once you have already installed the Azure CLI, you can view the currently authenticated account name with the az account show command:

```bash
az account show --query "{ subscription_id: id, tenant_id: tenantId }"
```

The output should be similar to the following:

```json
{
  "subscription_id": "00000000-0000-0000-0000",
  "tenant_id": "00000000-0000-0000-0000"
}
```

## Azure provider configuration block
Below is the example for Azure provider configuration block:

```terraform

provider "azurerm" {
  features {}
}

```
The subscription_id and tenant_id values can be used in the provider configuration block.
