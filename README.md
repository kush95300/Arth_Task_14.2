# Task 14.2

## Description:

 Further in ARTH - Task 10 have to create an
Ansible playbook that will retrieve newContainer IP
and update the inventory. So that further Configuration
of Webserver could be done inside that Container.

## Solution

created playbook for this:

- aws_instance_with_webserver.yml : PLAYBOOK to create one instance
- credentials.safe   :  CONTAINS IAM credentials   it is a vault
- parameters.yml     :  CONTAINS parameters
- vault_pass         :  VAULT PASS
- inventory.txt      :  ansible inventory


<b>
Command : ansible-playbook --vault-pass-file vault_pass aws_instance_with_webserver.yml 
</b>

#NOTE: System should have pip and ansible before running this playbook. 

Thank You 


CREATER: Kaushal Soni

