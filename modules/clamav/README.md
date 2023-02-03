# clamav - AWS EC2-VPC Security Group Terraform module

## Usage

```hcl
module "clamav_security_group" {
  source = "terraform-aws-modules/security-group/aws//modules/clamav"

  # omitted...
}
```

All automatic values **clamav module** is using are available [here](https://github.com/terraform-aws-modules/terraform-aws-security-group/blob/master/modules/clamav/auto_values.tf).

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
