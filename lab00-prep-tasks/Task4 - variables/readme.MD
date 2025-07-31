# Task 4 – Create a Linux User with Ansible based on variable

This Ansible playbook creates a Linux user using a variable and sets up a test directory inside the user's home folder.

## Steps:

- Creates a user based on the `user_name` variable
- Ensures the user has a home directory
- Creates a `testDIR` folder in `/home/<user_name>/`
- Uses `become: true` for privilege escalation

##  Usage

Run the playbook with:

```bash
ansible-playbook -i inventory main.yml --ask-become-pass
