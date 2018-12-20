# arch_server_basic

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

## Done
* install default packages: zsh, git, vim

## TODO (no particular order):
* fix shell
* install standard packages
* zshrc
* create user
* configure user
* secure ssh, forbid root login
* install sudo
* suply pubkeys
* configure vim
* aur
* firewall
* update
