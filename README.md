# Teamcity server with Ansible

This set of roles includes:
* Teamcity itself. With default local worker.
* Nginx as frontend server
* PostgreSQL as database server
* Oracle Java7 with JDBC
* Postfix for outgoing mail, with OpenDKIM for signing
* IPTables for access restrictions

## Installation

1. Edit `inventory/group_vars/all.yml`
2. Run `ansible-playbook -i inventory/production playbook/site.yml`

## Steps after installation

1. Configure DNS records for SPF/DKIM
2. Configure Teamcity through it's web interface

Feel free to contact me if you have any questions.