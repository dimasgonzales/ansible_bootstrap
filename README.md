# Ansible Bootstrap

My collection of Ansible bootstrap playbooks.

## Dependecies

- `git`
- `ansible`
    - `ansible-pull`
    - Ansible Galaxy Roles and Collections
        - `requirements.yml`

### Git
Depending on the host OS you will need to use any available package manager to install the `git` CLI.

Good Luck future Dimas

### Ansible
You can install ansible with `pip`
**Core Ansible**
```
pip install ansible
```

**Ansible Roles and Collections**
```bash
ansible-galaxy install -r requirements.yml
```

- `libselinux-python3`
```bash
sudo yum install -y libselinux-python3
```
## Executing Ansible playbook

```bash
sudo ansible-pull -U git@github.com:dimasgonzales/ansible_bootstrap.git --ask-become-pass
```