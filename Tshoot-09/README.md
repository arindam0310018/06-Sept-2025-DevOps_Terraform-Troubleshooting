# Terraform Troubleshooting 09:-

I. __Below follows the Terraform Error:-__

```
PS C:\Users\ARINDAM.MITRA\Desktop\__CODE\ZI-ELK-Terraform\Terraform-Frontend\05-kv> C:\AM-Tools\terraform.exe init            
Initializing the backend...
Initializing modules...
╷
│ Error: Error loading state:
│     executing request: Put "https://zi4np4dv4elk4infrareq4sa.blob.core.windows.net/terraform/05-kv/kv.tfstate": HTTP response was nil; connection may have been reset
│
│ Terraform failed to load the default state from the "azurerm" backend.
│ State migration cannot occur unless the state can be loaded. Backend
│ modification and state migration has been aborted. The state in both the
│ source and the destination remain unmodified. Please resolve the
│ above error and try again.

```

| RESOLUTION:- |
| --------- |
