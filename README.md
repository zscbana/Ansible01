# Ansible01 Repository

## Overview
This repository contains two assignments focused on setting up an **Nginx web server** using **Ansible**. Each assignment explores different methods of deployment, including direct playbook execution and structured **Ansible roles**.

## 📂 Repository Structure
```
Ansible01/
├── assignment01/
│   ├── README.md  # Details about Assignment 1
│   ├── inventory  # Ansible inventory file
│   ├── playbook.yml  # Ansible playbook for setting up Nginx
│   ├── nginx.conf.j2  # Jinja2 template for Nginx configuration
│   ├── PlayBook.png  # Screenshot of the playbook execution
│   └── other related files
│
├── assignment02/
│   ├── README.md  # Details about Assignment 2
│   ├── inventory  # Ansible inventory file
│   ├── playbook.yml  # Ansible playbook with Ansible roles
│   ├── roles/  # Ansible role for Nginx setup
│   │   ├── tasks/
│   │   ├── templates/
│   │   ├── handlers/
│   │   ├── defaults/
│   │   └── other role-related files
│   ├── PlayBook.png  # Screenshot of the playbook execution
│   └── other related files
```

## Assignments

### 📌 Assignment 1: Nginx Setup with Multipass and Ansible
- Created a new **virtual machine** using **Multipass**.
- Configured an **Ansible playbook** to install and configure **Nginx**.
- Restricted access to specific **IP addresses** using **Jinja2 templates**.
- [📄 Read More](https://github.com/zscbana/Ansible01/tree/main/Assignment01)

### 📌 Assignment 2: Nginx Setup with Ansible Roles
- Implemented the same **Nginx setup** but structured it using **Ansible roles**.
- Created a reusable **Ansible role** for automated Nginx configuration.
- Improved maintainability and **scalability** of the deployment.
- [📄 Read More](./assignment02/README.md)

## Requirements
- **Multipass** installed and configured.
- **Ansible** installed and configured.
- **SSH access** to target machines.
- Proper **privilege escalation** (`become: true`) for Ansible tasks.

## Running the Playbooks
To execute the **Ansible playbooks**, navigate to the respective assignment folder and run:

```bash
ansible-playbook -i inventory playbook.yml
```

## Conclusion
This repository showcases two approaches to deploying **Nginx with Ansible**. The **first assignment** focuses on using a straightforward playbook, while the **second assignment** demonstrates the power of **Ansible roles** for better organization and reusability.
