# Terraform Troubleshooting 08:-

I. __Below follows the Terraform Error:-__

```
Error: creating Agent Pool (Subscription: "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
│ Resource Group Name: "zi-np-appl-elk-dev-rg"
│ Managed Cluster Name: "zi-np-appl-elk-dev-aks"
│ Agent Pool Name: "main"): performing CreateOrUpdate: unexpected status 400 (400 Bad Request) with response: {
│   "code": "ErrCode_InsufficientVCPUQuota",
│   "details": null,
│   "message": "Insufficient vcpu quota requested 24, remaining 6 for family standardEASv4Family for region northeurope. If you want to increase the quota, please follow this instruction: https://learn.microsoft.com/en-us/azure/quotas/view-quotas. Surge nodes would also consume vcpu quota, please consider use smaller maxSurge or use maxUnavailable to proceed upgrade without surge nodes, details: aka.ms/aks/maxUnavailable.",
│   "subcode": ""
│  }
│ 
│   with module.aks.azurerm_kubernetes_cluster_node_pool.worker["main"],
│   on ../../Terraform-Backend/azurerm_kubernetes_cluster/aks-nodepools.tf line 8, in resource "azurerm_kubernetes_cluster_node_pool" "worker":
│    8: resource "azurerm_kubernetes_cluster_node_pool" "worker" {
│ 
╵

##[error]Script failed with exit code: 1
```

| RESOLUTION:- |
| --------- |
