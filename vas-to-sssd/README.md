Role Name
=========

vas-to-sssd

Requirements
------------

TBD

Role Variables
--------------

realm_permit_group = The standard "U-HOSTNAME-NIX" "Hag" plus the appropriate -vasg secondary group (such as hqUS-non-prod-vasg for USLI non-prod systems)

Dependencies
------------

The vault password will be communicated during the project.

Example Playbook
----------------

Execute as follows:
  ansible-playbook -b -i "inventory" main.yml --ask-vault-pass -e "realm_permit_group='U-{{ ansible_hostname }}-NIX,[hq|mi]US-[non-]prod-vasg'"

License
-------

UNLICENSED - ALL RIGHTS RESERVED(c)

Author Information
------------------

