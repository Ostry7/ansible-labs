# 🧰 Ansible Skeleton Project

This project provides a clean, modular Ansible project skeleton ready for use in real-world infrastructure automation scenarios.  
It includes a sample role `nginx_static_site` and a structure for future playbooks, variables, and environment-specific configurations.

## 📁 Project Structure

ansible-skeleton/
├── inventory/
│ ├── group_vars/ # Variables shared across host groups
│ └── host_vars/ # Host-specific variables
├── playbooks/ # Main playbooks go here
└── roles/
└── nginx_static_site/
├── defaults/ # Default role variables
├── files/ # Static files to copy
├── handlers/ # Handlers (e.g., for service restarts)
├── meta/ # Role dependencies and metadata
├── tasks/ # Main tasks
├── templates/ # Jinja2 templates for dynamic configuration
└── vars/ # High-priority role variables


## 🚀 How to Run the Playbook

Example execution (assuming `main.yml` is located in `playbooks/`):

```bash
ansible-playbook -i inventory playbooks/main.yml