# Terraform Troubleshooting 02:-

Greetings my fellow Technology Advocates and Specialists.

In this Terraform Troubleshooting Session, I will demonstrate, how I resolved the below encountered error - "Error acquiring the state lock. state blob is already locked"

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
| Unlock the Terraform State file located in the respective Storage Account. User needs to break the Terraform State File "Lease". | 
| The Terraform State file got locked beacaue the Terraform execution got cancelled because of below possible reasons:- |
| 1. Pipeline executing Terraform got timeout. |
| 2. User is running Terraform "Init", "Plan" and "Apply" manually over commandline. While "Apply" is "In-Progress", User terminates by pressing "Ctrl + C" |

__Hope You Enjoyed the Troubleshooting Session!!!__

__Stay Safe | Keep Learning | Spread Knowledge__
