## General Commands

List all hosts
```shell
ansible all --list-hosts
```
    
Gather system facts about all hosts
```shell
ansible all -m gather_facts
```
    
Gather facts for a single host (by IP or alias)
```shell
ansible all -m gather_facts --limit 192.168.1.10
```
    
## Playbooks

Run the playbook with:
```
ansible-playbook playbooks/site.yml
```

You can add flags:
- -v or -vvv for verbose output.
- --check (dry run) to see what changes would be made without applying them. 

This executes the tasks on all target hosts defined in your inventory.