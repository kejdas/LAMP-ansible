# LAMP-Ansible

This repository provides Ansible playbooks to automate the installation and configuration of a LAMP stack (Linux, Apache, MySQL, PHP) on Debian-based systems. It also includes configurations for setting up MySQL master-slave replication and deploying WordPress.

## Features

- **LAMP Stack Installation**: Automates the setup of Apache, MySQL, and PHP.
- **MySQL Master-Slave Replication**: Configures replication between master and slave databases.
- **WordPress Deployment**: Installs and configures WordPress with the LAMP stack.

## Prerequisites

- Debian-based system (e.g., Debian, Ubuntu).
- Ansible installed on the control machine.
- SSH access to target servers with a valid private key.
- Root or sudo privileges on target servers.

## Repository Structure

- `lamp_install.yml` - Playbook for installing the LAMP stack.
- `master_replication.yml` - Configures the master MySQL server for replication.
- `slave_replication.yml` - Sets up the slave MySQL server to replicate from the master.
- `wordpress_install.yml` - Installs and configures WordPress.
- `wordpress_db.yml` - Sets up the WordPress database.
- `hosts` - Inventory file defining target hosts.
- `vars/` - Directory containing variable files.
- `secrets.yml` - File for sensitive data (ensure this is secured).

## Usage

### 1. Clone the Repository

```bash
git clone https://github.com/kejdas/LAMP-ansible.git
cd LAMP-ansible
