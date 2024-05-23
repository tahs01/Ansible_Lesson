### Essential Commands

```bash
$ sudo ansible all -i hosts -m ping                                      #ping test to hosts
$ sudo ansible-playbook day_01_playbook.yml                              #run ansible playbook

$ sudo ansible-playbook day_02_playbook_with_cmd.yml --check             #check errors in playbook
$ sudo ansible-playbook day_02_playbook_with_cmd.yml --check --diff
$ sudo ansible-playbook day_02_playbook_with_cmd.yml --syntax-check

$ sudo ansible-vault create vault.yml                                    #create secrets variable with vault                   
New Vault password: 
Confirm New Vault password:

$ sudo ansible-vault edit vault.yml                                      #edit secrets variable with vault                              
Vault password:

$ sudo ansible-playbook day_02_playbook_with_module_pri_repo.yml --ask-vault-pass  
Vault password: 
(or)
$ sudo ansible-playbook day_02_playbook_with_module_pri_repo.yml --ask-vault-pass --ask-become-pass