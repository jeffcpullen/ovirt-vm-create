# Requirements

Needs python-ovirt-engine-sdk4

Requires credentials to your RHV instance. You can pass the credentials as variables or as environmental variables.


# Defaults

ovirt_wait: "True"
ovirt_cluster: "Default"
ovirt_name: "rhv-ocp-master"
ovirt_domain_name: "example.com"
ovirt_rhv_template: "rhel-server-7.7-template"
ovirt_dns_search: "example.com"
ovirt_nic_boot_protocol: "static"
ovirt_nic_ip_address: "192.168.1.5"
ovirt_nic_netmask: "255.255.255.0"
ovirt_nic_gateway: "192.168.1.1"
ovirt_nic_name: "eth0"
ovirt_nic_on_boot: "true"
openshift_cpu_cores: 2
openshift_memory: 4096MiB
ovirt_count: 1
ovirt_vm_disk_storage_domain: "nas-1tbssd"

