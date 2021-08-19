# Ansible Playbook to enable syslog on NXOS/IOS/IOS XE devices.

## How to use

1.  Install cisco.nxos collection
```shell
ansible-galaxy collection install cisco.nxos
```
2. Modify the inventory.ini
3. Run playbook
```shell
ansible-playbook set_syslog.yaml -i inventory.ini
```