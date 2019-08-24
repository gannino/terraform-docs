# Terraform Tools 

## Installers 

### Terraform Switcher - tfswitch

Installation and use. [Docs](https://github.com/warrensbox/terraform-switcher/)
```
curl -L https://raw.githubusercontent.com/warrensbox/terraform-switcher/release/install.sh | sudo bash
sudo chown -R $USER /usr/local/bin
tfswitch
```

If running into permissions issues then switch to user install and fix path
```
mkdir ~/bin
export PATH=$PATH:~/bin
tfswitch -b ~/bin/terraform
```

### Terragrunt Switcher - tgswitch

Installation and use. [Docs](https://github.com/warrensbox/tgswitch/)
```
curl -L https://raw.githubusercontent.com/warrensbox/terraform-switcher/release/install.sh | sudo bash
sudo chown -R $USER /usr/local/bin
tfswitch
```

## Converters 

### Compost 

- [Github](https://github.com/mootpt/compost)

Convert Terraform state to Pulumi State [WIP]


## Helpers 

### goat 

- [Github](https://github.com/sevagh/goat)
- [TF Example](https://github.com/sevagh/goat/tree/master/terraform-example)

goat is a Go program which runs from inside the EC2 instance.

By setting your tags correctly, goat can discover and attach EBS volumes and ENIs. For EBS volumes, 
it can perform additional actions such as RAID (with mdadm), mkfs, and mount EBS volumes to the EC2 
instance where it's running.
