# Qwiklab: Automating the Deployment of Infrastructure Using Terraform
<p align="center"><img src="infra.png" width="700px"></p>

# Usage
## rewrite the Terraform configuration files to a canonical format and style
```
terraform fmt

> OUTPUT
mynetwork.tf
```
## initialize Terraform
```
terraform init

> OUTPUT
Initializing modules...
- mynet-eu-vm in instance
- mynet-us-vm in instance
...
* provider.google: version = "~> 3.37"

Terraform has been successfully initialized!
```
## create an execution plan
```
terraform plan

> OUPUT
...
Plan: 4 to add, 0 to change, 0 to destroy.
...
```

## apply the desired changes
```
terraform apply

> TYPE
yes

> OUTPUT
...
Apply complete! Resources: 4 added, 0 changed, 0 destroyed.
```

## destroy resource
```
terraform destroy -auto-approve
```
