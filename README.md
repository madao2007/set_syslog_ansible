# Ansible Playbook to enable syslog on NXOS/IOS/IOS XE devices.

## How to use

1.  Install cisco.nxos and cisco.ios collection
```shell
ansible-galaxy collection install cisco.nxos
ansible-galaxy collection install cisco.ios
```
2. Modify the inventory.ini
3. Add `host_key_checking = False` to `/etc/ansible/ansible.cfg`
```shell
echo "host_key_checking = False" >> /etc/ansible/ansible.cfg
```
4. Modify the vars `syslog_server` in `group_vars/all.yaml`
5. Run playbook
```shell
ansible-playbook set_syslog.yaml -i inventory.ini
```

## In Belgium branch, to develop the Ansible jump host function