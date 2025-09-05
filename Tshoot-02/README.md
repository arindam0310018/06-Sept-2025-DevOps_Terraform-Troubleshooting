# Terraform Troubleshooting 02:-

I. __Below follows the Terraform Error:-__

```
Error: Error acquiring the state lock

Error message: state blob is already locked
Lock Info:
  ID:        a885db42-468e-73be-71a8-c17ad290779f
  Path:      terraform/08-aks/aks.tfstate
  Operation: OperationTypeApply
  Who:       root@am-dev-linux-placeholder-84c7db67d4-hlkcj
  Version:   1.9.6
  Created:   2025-09-01 14:33:40.335739467 +0000 UTC
  Info:      


Terraform acquires a state lock to protect the state from being written
by multiple users at the same time. Please resolve the issue above and try
again. For most commands, you can disable locking with the "-lock=false"
flag, but this is not recommended.

##[error]Script failed with exit code: 1

```

| RESOLUTION:- |
| --------- |
