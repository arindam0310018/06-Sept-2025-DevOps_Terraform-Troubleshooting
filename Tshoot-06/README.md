# Terraform Troubleshooting 06:-

I. __Below follows the Terraform Error:-__

```
╷
│ Error: `max_count` and `min_count` must be set to `null` when auto_scaling_enabled is set to `false`
│ 
│   with module.aks.azurerm_kubernetes_cluster_node_pool.worker["kafka"],
│   on ../../Terraform-Backend/azurerm_kubernetes_cluster/aks-nodepools.tf line 8, in resource "azurerm_kubernetes_cluster_node_pool" "worker":
│    8: resource "azurerm_kubernetes_cluster_node_pool" "worker" {
│ 
╵
```

| RESOLUTION:- |
| --------- |
