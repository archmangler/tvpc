# AWS VPC module for Terraform

A lightweight VPC module for Terraform.

## Usage

```hcl
module "vpc" {
  source = "./vpc"

  environment = "vpc_name"
  key_name = "osadmin"

  vpc_cidr = "10.0.0.0/16"
  public_subnets = ["10.0.1.0/24"]
  private_subnets = ["10.0.100.0/24"]
}
```

See `interface.tf` for additional configurable variables.

## License

MIT

