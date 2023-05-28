# [azure_cli](#azure_cli)

Install and configure azure_cli on your system.

|GitHub|GitLab|Quality|Downloads|Version|Issues|Pull Requests|
|------|------|-------|---------|-------|------|-------------|
|[![github](https://github.com/buluma/ansible-role-azure_cli/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-azure_cli/actions)|[![gitlab](https://gitlab.com/shadowwalker/ansible-role-azure_cli/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-azure_cli)|[![quality](https://img.shields.io/ansible/quality/59165)](https://galaxy.ansible.com/buluma/azure_cli)|[![downloads](https://img.shields.io/ansible/role/d/59165)](https://galaxy.ansible.com/buluma/azure_cli)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-azure_cli.svg)](https://github.com/buluma/ansible-role-azure_cli/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-azure_cli.svg)](https://github.com/buluma/ansible-role-azure_cli/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-azure_cli.svg)](https://github.com/buluma/ansible-role-azure_cli/pulls/)|

## [Example Playbook](#example-playbook)

This example is taken from [`molecule/default/converge.yml`](https://github.com/buluma/ansible-role-azure_cli/blob/master/molecule/default/converge.yml) and is tested on each push, pull request and release.

```yaml
---
- name: converge
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - role: buluma.azure_cli
```

The machine needs to be prepared. In CI this is done using [`molecule/default/prepare.yml`](https://github.com/buluma/ansible-role-azure_cli/blob/master/molecule/default/prepare.yml):

```yaml
---
- name: prepare
  hosts: all
  become: yes
  gather_facts: no

  roles:
    - role: buluma.bootstrap
    - role: buluma.epel
    - role: buluma.buildtools
    - role: buluma.python_pip
    - role: buluma.microsoft_repository_keys
```

Also see a [full explanation and example](https://buluma.github.io/how-to-use-these-roles.html) on how to use these roles.


## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-azure_cli/blob/master/requirements.txt).

## [State of used roles](#state-of-used-roles)

The following roles are used to prepare a system. You can prepare your system in another way.

| Requirement | GitHub | GitLab |
|-------------|--------|--------|
|[buluma.bootstrap](https://galaxy.ansible.com/buluma/bootstrap)|[![Build Status GitHub](https://github.com/buluma/ansible-role-bootstrap/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-bootstrap/actions)|[![Build Status GitLab](https://gitlab.com/shadowwalker/ansible-role-bootstrap/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-bootstrap)|
|[buluma.buildtools](https://galaxy.ansible.com/buluma/buildtools)|[![Build Status GitHub](https://github.com/buluma/ansible-role-buildtools/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-buildtools/actions)|[![Build Status GitLab](https://gitlab.com/shadowwalker/ansible-role-buildtools/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-buildtools)|
|[buluma.epel](https://galaxy.ansible.com/buluma/epel)|[![Build Status GitHub](https://github.com/buluma/ansible-role-epel/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-epel/actions)|[![Build Status GitLab](https://gitlab.com/shadowwalker/ansible-role-epel/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-epel)|
|[buluma.microsoft_repository_keys](https://galaxy.ansible.com/buluma/microsoft_repository_keys)|[![Build Status GitHub](https://github.com/buluma/ansible-role-microsoft_repository_keys/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-microsoft_repository_keys/actions)|[![Build Status GitLab](https://gitlab.com/shadowwalker/ansible-role-microsoft_repository_keys/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-microsoft_repository_keys)|
|[buluma.python_pip](https://galaxy.ansible.com/buluma/python_pip)|[![Build Status GitHub](https://github.com/buluma/ansible-role-python_pip/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-python_pip/actions)|[![Build Status GitLab](https://gitlab.com/shadowwalker/ansible-role-python_pip/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-python_pip)|

## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-azure_cli/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|[Alpine](https://hub.docker.com/repository/docker/buluma/alpine/general)|all|
|[EL](https://hub.docker.com/repository/docker/buluma/enterpriselinux/general)|8|
|[Debian](https://hub.docker.com/repository/docker/buluma/debian/general)|bullseye|
|[Fedora](https://hub.docker.com/repository/docker/buluma/fedora/general)|all|
|[Ubuntu](https://hub.docker.com/repository/docker/buluma/ubuntu/general)|all|

The minimum version of Ansible required is 2.10, tests have been done to:

- The previous version.
- The current version.
- The development version.

If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-azure_cli/issues)

## [Changelog](#changelog)

[Role History](https://github.com/buluma/ansible-role-azure_cli/blob/master/CHANGELOG.md)

## [License](#license)

[Apache-2.0](https://github.com/buluma/ansible-role-azure_cli/blob/master/LICENSE).

## [Author Information](#author-information)

[buluma](https://buluma.github.io/)

Please consider [sponsoring me](https://github.com/sponsors/buluma).

### [Special Thanks](#special-thanks)

Template inspired by [Robert de Bock](https://github.com/robertdebock)
