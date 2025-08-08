# Task 6 - Delete user with Ansible using vars (multiple variables)

This Ansible playbook deletes users on Linux hosts using variables specified in `roles/delete-user/vars/vars.yml`, with conditional group assignment based on OS family. The script loops the deletion activity based on the number of usernames.

The playbook `main.yml`:

    Delete user[0]++ on Linux hosts

    Uses privilege escalation (become: true) to perform user creation

## Usage

To run the playbook:

```bash
ansible-playbook -i inventory main.yml --ask-become-pass