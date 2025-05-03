# PVE Ansible Setup

### This is a collection of Ansible playbooks and roles to automate the setup of a Proxmox VE (PVE) environment.

## Installation

### To install the required dependencies, run the following command:

```bash
pip install ansible ansible-lint ansible-vault
```

### To install the required Ansible collections, run the following command:

```bash
ansible-galaxy collection install -r requirements.yml
```

## Inventory

Update the inventory file with the IP addresses of your Proxmox nodes. The inventory file is located at `inventory.yml`.

## Group Variables

The group variables for the Proxmox nodes are located in `group_vars/all.yml`. Update the variables as needed.

### Example Variables

- `pve_user`: The username for Proxmox access.
- `pve_password`: The password for Proxmox access.

## Playbooks

The playbooks are located in the `playbooks` directory. Each playbook is responsible for a specific task.

- os_updates.yml: Updates the operating system on all Proxmox nodes and VMs and LXCs.
