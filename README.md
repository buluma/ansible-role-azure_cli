# [Ansible role azure_cli](#ansible-role-azure_cli)

Install and configure azure_cli on your system.

|GitHub|GitLab|Downloads|Version|
|------|------|---------|-------|
|[![github](https://github.com/buluma/ansible-role-azure_cli/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-azure_cli/actions)|[![gitlab](https://gitlab.com/shadowwalker/ansible-role-azure_cli/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-azure_cli)|[![downloads](https://img.shields.io/ansible/role/d/buluma/azure_cli)](https://galaxy.ansible.com/buluma/azure_cli)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-azure_cli.svg)](https://github.com/buluma/ansible-role-azure_cli/releases/)|

## [Example Playbook](#example-playbook)

This example is taken from [`molecule/default/converge.yml`](https://github.com/buluma/ansible-role-azure_cli/blob/master/molecule/default/converge.yml) and is tested on each push, pull request and release.

```yaml
  - name: Converge
    hosts: all
    become: yes
    gather_facts: yes

    roles:
      - role: buluma.azure_cli
```

The machine needs to be prepared. In CI this is done using [`molecule/default/prepare.yml`](https://github.com/buluma/ansible-role-azure_cli/blob/master/molecule/default/prepare.yml):

```yaml
  - name: Prepare
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

This role is part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:
![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-azure_cli/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|[Alpine](https://hub.docker.com/r/buluma/alpine)|all|
|[EL](https://hub.docker.com/r/buluma/enterpriselinux)|all|
|[Debian](https://hub.docker.com/r/buluma/debian)|all|
|[Fedora](https://hub.docker.com/r/buluma/fedora)|all|
|[Ubuntu](https://hub.docker.com/r/buluma/ubuntu)|all|

The minimum version of Ansible required is 2.12, tests have been done on:

- The previous version.
- The current version.
- The development version.

If you find issues, please register them on [GitHub](https://github.com/buluma/ansible-role-azure_cli/issues).

## [License](#license)

[Apache-2.0](https://github.com/buluma/ansible-role-azure_cli/blob/master/LICENSE).

## [Author Information](#author-information)

[buluma](https://buluma.github.io/)

