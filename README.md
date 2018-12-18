#### terraform-libvirt-cloudinit
Simple example of using terraform with libvirt plugin.

### Overview
Using Terraform to setting a cluster of N identical local QEMU virtual machines.

### Enviroment
Tested on:
* Ubuntu 18.04
* Terraform 0.11.10

### Installation
TBD

### Usage
```
After pulling and modifying .tf files init terraform and tell it to load modules etc.
terraform init

Create plan of how to change enviroment
terraform plan -out=terraplan

You can also define number of insances
TF_NUMBER_OF_INSTANCES=5 terraform plan -out=terraplan

Apply plan and execute it
terraform apply terraplan
```
```
You can destroy all created resources with
terraform destroy
```
### Sources
Created (not so easy) based on:
* https://titosoft.github.io/kvm/terraform-and-kvm/ (some things not actual)
* https://www.terraform.io/docs/configuration/interpolation.html
* https://github.com/dmacvicar/terraform-provider-libvirt/blob/master/examples/count/main.tf
* https://github.com/dmacvicar/terraform-provider-libvirt/blob/master/website/docs/r
