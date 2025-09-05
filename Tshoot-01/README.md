# Terraform Troubleshooting 01:-

I. __Below follows the Terraform Error:-__

```
Error: creating Kubernetes Cluster (Subscription: "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
│ Resource Group Name: "zi-np-appl-elk-dev-rg"
│ Kubernetes Cluster Name: "zi-np-appl-elk-dev-aks"): performing CreateOrUpdate: unexpected status 400 (400 Bad Request) with response: {
│   "code": "ExistingRouteTableNotAssociatedWithSubnet",
│   "details": null,
│   "message": "An existing route table has not been associated with subnet /subscriptions/xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx/resourceGroups/elkei-dev-vnet-rg/providers/Microsoft.Network/virtualNetworks/elkei-dev-vnet/subnets/zi-np-elk-dev-aks-sn. Please update the route table association",
│   "subcode": ""
│  }
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
