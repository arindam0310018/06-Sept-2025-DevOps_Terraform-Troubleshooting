# Terraform Troubleshooting 03:-

Greetings my fellow Technology Advocates and Specialists.

In this Terraform Troubleshooting Session, I will demonstrate, how I resolved the below encountered error - "A resource with the ID already exists - to be managed via Terraform this resource needs to be imported into the State."

| I. __TERRAFORM ERROR 03:-__ |
| :--------- |

```
╷
│ Error: A resource with the ID "/subscriptions/xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx/resourceGroups/zi-np-appl-elk-dev-rg/providers/Microsoft.ContainerService/managedClusters/zi-np-appl-elk-dev-aks" already exists - to be managed via Terraform this resource needs to be imported into the State. Please see the resource documentation for "azurerm_kubernetes_cluster" for more information.
│ 
│   with module.aks.azurerm_kubernetes_cluster.aks,
│   on ../../Terraform-Backend/azurerm_kubernetes_cluster/aks.tf line 52, in resource "azurerm_kubernetes_cluster" "aks":
│   52: resource "azurerm_kubernetes_cluster" "aks" {
│ 
╵

##[error]Script failed with exit code: 1

```

| II. __WHY THE ERROR WAS ENCOUNTERED:-__ |
| :--------- |
| 1. This Error was encountered because Pipeline executing Terraform got timeout. |

| III. __RESOLUTION:-__ |
| :--------- |
| 1. Delete the respective resource, here for example is "AKS" using Powershell, Az CLI, or over Azure Portal. Then, Re-Run the pipeline executing Terraform or Run Terraform commands manually over Terminal. | 

__Hope You Enjoyed the Troubleshooting Session!!!__

__Stay Safe | Keep Learning | Spread Knowledge__
