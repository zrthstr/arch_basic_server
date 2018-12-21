# arch_server_basic

## usage

### overwrite `default_packages`:
```
## playbook/play.yml
- hosts: rand
  roles:
    - role: arch_basic_server
      admin_acc: "some_name"
      admin_acc: "/home/some_local_name/.ssh/id_rsa.pub"
      packages:
        - vim
        - gcc
```

## Done
* install default packages: zsh, git, vim
* fix shell
* grml-zshrc
* create user
* configure user
* install sudo
* suply pubkeys
* secure ssh, forbid root login
* configure vim

## TODO (no particular order):
* aur
* firewall
* auto update?
