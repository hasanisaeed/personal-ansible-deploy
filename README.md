# personal-ansible-deploy

This is my personal Ansible configuration for deployment.

It includes:

1. Project directory structure for Ansible  
2. Ansible configuration files (`ansible.cfg`, `hosts.ini`, `group_vars`)  
3. Roles for Backend and Frontend  
4. The main Playbook  
5. Tag usage to run only Backend or Frontend  
6. Sample GitHub Actions workflow to run Ansible after build  

---

## 1. Directory Structure

```text
ansible-deploy/
├── ansible.cfg
├── hosts.ini
├── group_vars/
│   ├── production.yml
│   └── staging.yml
├── playbook.yml
└── roles/
    ├── backend/
    │   ├── vars/main.yml
    │   └── tasks/main.yml
    └── frontend/
        ├── vars/main.yml
        └── tasks/main.yml

