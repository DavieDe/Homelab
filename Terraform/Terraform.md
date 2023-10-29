# Terraform Documentation

- <https://github.com/bpg/terraform-provider-proxmox/blob/main/README.md>

- Install homebrew if not installed

- Install terrform

- Install tfenv

- Use tfenv to install terraform 1.5.5 (tfenv install 1.5.5)

- In the Terraform provider you want to add a required version for 1.5.5 . This version of terraform is compatible with Tofu which will be used when not in alpha
`
    terraform {
  required_version = "= 1.5.5"
`

- The folder strucutre should be
    Enviorment
        Production
            vm/other services in their own folders
        terraform.tfvars
    Modules
        module for vms or other services