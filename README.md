# Ansible EC2 HTTPD Deploy

This project automates the deployment of an EC2 instance on AWS and installs an Apache HTTP server (`httpd`) with a custom `index.html` page using Ansible.

---

## 🚀 Project Workflow

### 1. Prerequisites

- AWS account with access keys
- IAM user with permissions for EC2
- Python 3.x installed
- Ansible installed (`pip install ansible`)
- Boto3 and Botocore installed (`pip install boto3 botocore`)
- SSH key pair for EC2 access
- Ansible EC2 dynamic inventory plugin enabled

---

### 2. Directory Structure

ansible-ec2-httpd-deploy/
├── ansible.cfg
├── inventory/
│ └── aws_ec2.yaml
├── playbooks/
│ ├── create_ec2.yaml
│ └── setup_httpd.yaml
├── vars/
│ └── aws_ec2_variables.yaml
├── app/
│ └── index.html
├── roles/ (optional, for scaling later)
├── README.md
