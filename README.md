# Ansible Skel

Skeleton structure for repositories holding Ansible-managed hosts configuration.

## Usage

Download the latest release tarball at https://github.com/mtpereira/ansible-skel/releases/latest.

## Directory structure

- `group_vars`: Place group variables here. Splitting variables on multiple
  `.yml` files according to role name, organized on group-named directories
   (e.g., `group_vars/webserver/nginx.yml`) is highly recommended.
- `host_vars`: Place host specific variables here, in the same fashion as
   `group_vars` (e.g., `host_vars/web1/nginx.yml`. Always prefer placing
   variables on `group_vars`.
- `roles`: Directory where `ansible-galaxy` will place the roles required by
   `requirements.yml`.
- `files:` Place files for `copy` and `template` tasks here.

## TODO

- [X] Directory structure
- [ ] Vagrantfile
- [ ] ansible.cfg
- [ ] Makefile
- [ ] requirements.yml for roles
- [ ] requirements.txt for pip/virtualenv
- [ ] Template all the things!

