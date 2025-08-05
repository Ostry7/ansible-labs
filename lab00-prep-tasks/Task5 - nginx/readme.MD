# Task 5 – Deploy a custom Nginx site with Ansible

This Ansible playbook installs Nginx and deploys a custom site configuration using a Jinja2 template.

**Steps:**

- Installs Nginx if not already present  
- Creates a document root directory (`document_root`)  
- Deploys an Nginx config from `nginx.conf.j2`  
- Enables the site by creating a symlink in `sites-enabled`  
- Disables the default Nginx site  
- Creates a simple `index.html` page  
- Reloads Nginx to apply changes  

**Usage**

Run the playbook with:

```bash
ansible-playbook -i inventory main.yml --ask-become-pass -e "server_name=example.local document_root=/var/www/example"
```
