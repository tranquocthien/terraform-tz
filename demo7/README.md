# Demo 7

```
cd demo7

terraform version
## Output: Terraform v0.12.19

terraform init

terraform workspace new Development

terraform plan -out dev.tfplan

terraform apply "dev.tfplan"

terraform workspace new UAT

terraform plan -out uat.tfplan

terraform apply "uat.tfplan"

terraform workspace new Production

terraform plan -out prod.tfplan

terraform apply "prod.tfplan"

terraform workspace list

## To switch to another workspace
terraform workspace select Development

terraform output

terraform destroy
```