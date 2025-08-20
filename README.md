# 🛠️ Ansible Labs – Learning Projects

This repository contains a series of hands-on projects for learning **Ansible** as part of my journey into DevOps. Each directory includes a self-contained scenario that demonstrates specific Ansible features or use cases.

---

## 📚 Project List

### 01. Basic Nginx Setup

* **Goal:** Learn basic modules: `apt/yum`, `service`, `copy`, `template`.
* **Description:** Install and configure Nginx using a custom configuration file.

### 02. Developer Environment Setup

* **Goal:** Automate installation of essential dev tools (Git, Docker, Zsh, etc.).
* **Description:** Create a `devtools` role to provision a new developer VM.

### 03. Nextcloud Installation

* **Goal:** Automate installation of Nextcloud with all dependencies and proper web server configuration.
* **Description:** Use the `nextcloud-install` role to:

  * Install required packages (Apache2, MariaDB, PHP modules, utilities)
  * Create database and user for Nextcloud
  * Download and install specified Nextcloud version
  * Configure Apache2 using a Jinja2 template
  * Enable necessary Apache modules and set correct file permissions
  * Start Nextcloud service and provide URL for browser access

---

## 📌 Purpose

This repository is my personal lab to:

* Practice real-world Ansible automation
* Learn DevOps workflows and IaC
* Build a portfolio of practical projects

---

> 🚀 Work in progress. More coming soon.
