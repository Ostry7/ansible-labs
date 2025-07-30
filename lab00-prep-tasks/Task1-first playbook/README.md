# Task1 - First Playbook

This is a simple Ansible playbook for testing a basic role.

The playbook `test.yml` runs the `test` role, which:

- Displays a test message with the hostname
- Runs a ping to check connectivity

To run the playbook:

```bash
ansible-playbook -i inventory test.yml
