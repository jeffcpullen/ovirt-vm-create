# Ansible Role: ovirt-vm-create

This role is designed to create virtual machines on ovirt/rhv using a few variables. combined with a loop it is simple to build out many disimiliar systems quickly

## Actions:

Actions performed by this role


#### Ovirt_auth:
* Obtain an SSO token
#### Ovirt_vm:
* Create the virtual machine on oVirt/RHV

## Tags:
## Variables:

* `ovirt_wait`: `"True"` - Decides if the play should wait for the vm creation to finish before moving on



* `ovirt_cluster`: `"Default"` - The name of the ovirt/RHV cluster to deploy in



* `ovirt_name`: `"rhv-ocp-master"` - The prefix for the deployed VM



* `ovirt_domain_name`: `"example.com"` - The domain that should be appended to the hostname for naming the VM



* `ovirt_rhv_template`: `"rhel-7.6-20190517-cloud"` - The template that should be used for deploying



* `ovirt_dns_search`: `"example.com"` - The dns search that should be added to the vm's /etc/resolv.conf



* `ovirt_nic_boot_protocol`: `"static"` - The network protocol for the VM



* `ovirt_nic_ip_address`: `"192.168.1.5"` - The IP address to be assigned for static NIC configs



* `ovirt_nic_netmask`: `"255.255.255.0"` - The netmask to be assigned for static NIC configs



* `ovirt_nic_gateway`: `"192.168.1.1"` - The vm's gateway to be assigned for static NIC configs



* `ovirt_nic_name`: `"eth0"` - The name to set for the network interface



* `ovirt_nic_on_boot`: `"true"` - If the network interface should be started at boot



* `openshift_cpu_cores`: `2` - The number of CPU cores to assign to the VM



* `openshift_memory`: `4096MiB` - The ammount of RAM to assign to the VM



* `ovirt_vm_disk_storage_domain`: `"nas-1tbssd"` - The storage domain name in ovirt/RHV



* `ovirt_insecure_login`: `True` - If certificates are trusted between the ansible host and oVirt/RHV this can be set to false


## TODO:

#### Improvement:


## Author Information
This role:  was created by: Jeff pullen
Jpullen@redhat.com
Documentation generated using: [Ansible-autodoc](https://github.com/AndresBott/ansible-autodoc)
