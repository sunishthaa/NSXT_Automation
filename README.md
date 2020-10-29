Ansible Tower NSX-T Automation
Synopsis
This Repository comprise of NSX-T Modules for Ansible. The Base module and library is forked from https://github.com/vmware/ansible-for-nsxt and any future library update should be synced with official VMware github side.

Prerequisites:
Ansible or Ansible tower Installed
Python3 >= 3.6.8
PyVmOmi - Python library for vCenter api.(install using— pip install —upgrade pyvmomi pyvim requests ssl)
OVF Tools - Ovftool is used for ovf deployment.(
https://www.virtual-odyssey.com/2017/11/26/install-vmware-ovftool-ubuntu/
https://my.vmware.com/web/vmware/downloads/details?downloadGroup=OVFTOOL430&productId=742 )
Test Environment Versions:
NSX-T 3.0.x
vSphere- 6.7
Ansible Tower- 3.7
Supported Reference URLs for Build:
Implementation Reference-
https://shuttletitan.com/nsx-t/nsx-t-installation-series/nsx-t-installation-series-step-0-high-level-design/
https://docs.vmware.com/en/VMware-NSX-T-Data-Center/index.html

Example:
---
- hosts: localhost
  roles:
    - nsxt_deploy_ova
Define yaml playbook in main directory calling required role
Adjust variable values in Groupvars
Run the playbook from Absible tower or Ansible control VM directly
