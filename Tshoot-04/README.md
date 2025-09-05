# Terraform Troubleshooting 04:-

I. __Below follows the Terraform Error:-__

```
│ Error: creating Kubernetes Cluster (Subscription: "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx")
│ Resource Group Name: "zi-np-appl-elk-dev-rg"
│ Kubernetes Cluster Name: "zi-np-appl-elk-dev-aks"): polling after CreateOrUpdate: polling failed: the Azure API returned the following error:
│ 
│ Status: "VMExtensionProvisioningError"
│ Code: ""
│ Message: "CSE failed with 'VMExtensionError_K8SAPIServerDNSLookupFail', which means agents are unable to resolve Kubernetes API server name. It's likely custom DNS server is not correctly configured, please see https://aka.ms/aks/vmextensionerror_k8sapiserverdnslookupfail and https://aka.ms/aks/private-cluster#hub-and-spoke-with-custom-dns for more information."
│ Activity Id: ""
│ 
│ ---
│ 
│ API Response:
│ 
│ ----[start]----
│ {
│  "name": "feafbb13-64ab-4c3f-abe1-8142ab169114",
│  "status": "Failed",
│  "startTime": "2025-09-02T11:35:09.0044412Z",
│  "endTime": "2025-09-02T11:49:18.4471253Z",
│  "error": {
│   "code": "VMExtensionProvisioningError",
│   "message": "CSE failed with 'VMExtensionError_K8SAPIServerDNSLookupFail', which means agents are unable to resolve Kubernetes API server name. It's likely custom DNS server is not correctly configured, please see https://aka.ms/aks/vmextensionerror_k8sapiserverdnslookupfail and https://aka.ms/aks/private-cluster#hub-and-spoke-with-custom-dns for more information."
│  }
│ }
│ -----[end]-----
│ 
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
