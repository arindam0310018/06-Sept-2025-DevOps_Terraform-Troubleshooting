# Terraform Troubleshooting 03:-

I. __Below follows the Terraform Error:-__

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

| RESOLUTION:- |
| --------- |
