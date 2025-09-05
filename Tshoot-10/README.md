# Terraform Troubleshooting 10:-

I. __Below follows the Terraform Error:-__

```
Error: creating/updating Virtual Network Link (Subscription: "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
│ Resource Group Name: "zi-np-appl-elk-dev-rg"
│ Private Dns Zone Name: "privatelink.vaultcore.azure.net"
│ Virtual Network Link Name: "kv-dns-link"): polling after CreateOrUpdate: polling failed: the Azure API returned the following error:
│
│ Status: "BadRequest"
│ Code: ""
│ Message: "A virtual network cannot be linked to multiple zones with overlapping namespaces. You tried to link virtual network with 'privatelink.vaultcore.azure.net' and 'privatelink.vaultcore.azure.net' zones."
│ Activity Id: ""
│
│ ---
│
│ API Response:
│
│ ----[start]----
│ {"error":{"code":"BadRequest","message":"A virtual network cannot be linked to multiple zones with overlapping namespaces. You tried to link virtual network with 'privatelink.vaultcore.azure.net' and 'privatelink.vaultcore.azure.net' zones."},"status":"Failed"}
│ -----[end]-----
│
│
│   with module.zi_key_vault.azurerm_private_dns_zone_virtual_network_link.keyvault_dns_link,
│   on ..\..\Terraform-Backend\azurerm_key_vault\keyvault.tf line 54, in resource "azurerm_private_dns_zone_virtual_network_link" "keyvault_dns_link":    
│   54: resource "azurerm_private_dns_zone_virtual_network_link" "keyvault_dns_link" {
```

| RESOLUTION:- |
| --------- |
