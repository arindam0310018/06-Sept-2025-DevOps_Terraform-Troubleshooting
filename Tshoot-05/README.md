# Terraform Troubleshooting 05:-

I. __Below follows the Terraform Error:-__

```
╷
│ Error: creating Agent Pool (Subscription: "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
│ Resource Group Name: "zi-np-appl-elk-dev-rg"
│ Managed Cluster Name: "zi-np-appl-elk-dev-aks"
│ Agent Pool Name: "main"): performing CreateOrUpdate: unexpected status 400 (400 Bad Request) with response: {
│   "code": "BadRequest",
│   "details": null,
│   "message": "The VM size of Standard_E8as_v4 is only allowed  in zones [2 1] in your subscription in location 'northeurope'. ",
│   "subcode": ""
│  }
│ 
│   with module.aks.azurerm_kubernetes_cluster_node_pool.worker["main"],
│   on ../../Terraform-Backend/azurerm_kubernetes_cluster/aks-nodepools.tf line 8, in resource "azurerm_kubernetes_cluster_node_pool" "worker":
│    8: resource "azurerm_kubernetes_cluster_node_pool" "worker" {
│ 
╵
```

| RESOLUTION:- |
| --------- |

