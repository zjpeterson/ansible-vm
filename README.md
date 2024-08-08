# ansible-vm

This is the Ansible code for a demo I do which provisions a VM on one of the following platforms depending on user requirement: AWS EC2, Azure VM, GCP CE, VMWare vSphere

It is able to get an IP for the new VM from Infoblox and update ServiceNow after the build.

## Dev info
Set environment variables:

```
export AWS_ACCESS_KEY=
export AWS_SECRET_ACCESS_KEY=
export INFOBLOX_HOST=
export INFOBLOX_USERNAME=
export INFOBLOX_PASSWORD=
export INFOBLOX_SSL_VERIFY=
export SN_HOST=
export SN_USERNAME=
export SN_PASSWORD=
```

Extra vars inputs:
```
-e vm_name=test1 -e vm_cloud=aws -e vm_size=small -e vm_os=linux-RHEL8 -e vm_disk_gb=80
-e vm_azure_rg: openenv-x -e vm_google_project: openenv-y -e vm_aws_subnet: subnet-z
```
