# Task 2 - Install htop with Ansible

This is a simple Ansible playbook for installing the `htop` package using a dedicated role.

The playbook `main.yml` runs the `install-htop` role, which:

- Installs the `htop` package on Linux hosts (depends on Linux version)
- Uses privilege escalation (`become: true`) if necessary

## Usage

To run the playbook:

```bash
ansible-playbook -i inventory main.yml
