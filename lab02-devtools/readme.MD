# Lab02 - Developer Environment setup (dev tools: Git, Docker, Zsh)

This is a simple Ansible playbook for installing the `Git`, `Docker` and `Zsh` apps using a dedicated role.

The playbook `main.yml` runs the `devtools` role, which:

- Installs the `Git` package on Linux hosts (depends on Linux version)
- Installs the `Docker` package on Linux hosts (depends on Linux version)
- Installs the `Zsh` package on Linux hosts (depends on Linux version)
- Uses privilege escalation (`become: true`) if necessary

## Usage

To run the playbook:

```bash
ansible-playbook -i inventory main.yml --ask-become-pass
