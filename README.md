# arch_basic_server

## usage

### overwrite `default_packages`:
```
## playbook/play.yml
- hosts: rand
  roles:
    - role: arch_basic_server
      packages:
        - vim
        - gcc
```
