# arch_server_basic

# first run

for running ansible in normal mode we first need to make sure python is
installed and some other quirks are taken care of.
This can be done with `first_run_inline_playbook_role/first.yml` and
should only be needed once.

example: `ansible-playbook -i inventory.foo some_path/first_run_inline_playbook_role/first.yml --user=root


## usage

```
## playbook/play.yml
- hosts: rand
  roles:
    - role: arch_basic_server
      admin_acc: "some_name"
      admin_acc: "/home/some_local_name/.ssh/id_rsa.pub"
## overwrite `default_packages`:
#      packages:
#        - vim
#        - gcc

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
* fix scaleway quirq: chmod 755 /usr /etc /usr/local /usr/local/sbin /usr/local/bin ...
