# Ansible Practice Lab

A compact collection of Ansible playbooks and roles for automating common Linux administration tasks.

## What is included

- Host connectivity checks and fact gathering
- Package installation and service management
- Apache installation and configuration
- File deployment and template-style configuration generation
- Reusable role examples under `roles/`

## Prerequisites

- Ansible installed on the control machine
- SSH access to the target hosts
- An inventory configured in `hosts.txt`

## Usage

```bash
ansible all -m ping
ansible-playbook playbook1.yml
```

Use the playbook that matches the scenario you want to test. Review its variables and target hosts before running it.

## Repository layout

```text
.
├── ansible.cfg
├── hosts.txt
├── playbook*.yml
├── All_in_one.yml
├── group_vars/
└── roles/
```

## Security

Do not commit real passwords, private keys, or production inventory data. Use [Ansible Vault](https://docs.ansible.com/ansible/latest/vault_guide/) or an external secrets manager for sensitive values.

> This repository is an educational lab. Validate every playbook before using it outside a disposable environment.
