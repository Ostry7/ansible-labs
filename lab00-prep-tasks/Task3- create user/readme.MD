Task 3 - Create testuser with Ansible

This is a simple Ansible playbook for creating a testuser on Linux hosts using conditional group assignment based on the OS family.

The playbook main.yml:

    Creates user testuser on Linux hosts

    Adds user to group sudo on Debian-based systems

    Adds user to group wheel on RedHat-based systems

    Uses privilege escalation (become: true) to perform user creation

Usage

To run the playbook:

ansible-playbook -i inventory main.yml --ask-become-pass