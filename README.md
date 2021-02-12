# TLDR

Ansible playbooks for ubuntu based distros.

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
