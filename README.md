# TLDR

Ansible playbooks for ubuntu based distros.

# Homelab playbooks

### pve-setup.yml
Creates user accounts, permissions, and everything else needed to access the host. See `Homelab Setup > Create the vault` to see how to setup the vault.

```
ansible-playbook --ask-vault-pass pve-setup.yml
```
# Homelab Setup


### Create the vault

```
ansible-vault create vault/pve
```

```yml
---
vaulted_pve_password: secret
```

# Facts

View your facts

```
ansible -m setup devmachine
```

# Roles

To create a new role, run the following command from this directory where `<role>` is the name of your new role.

```
ansible-galaxy init roles/<role>
```

# Thanks
* https://github.com/lae/ansible-role-proxmox
