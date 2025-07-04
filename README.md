# Ansible Role: asdf

[![CI](https://github.com/1000Bulbs/ansible-role-asdf/actions/workflows/ci.yml/badge.svg)](https://github.com/1000Bulbs/ansible-role-asdf/actions/workflows/ci.yml)

A brief description of the role goes here.

---

## Requirements

- Ansible 2.13+
- Python 3.9+ (for Molecule + testinfra)
- Tested on Ubuntu 22.04+

---

## Role Variables

These variables can be overridden in your inventory, playbooks, or `group_vars`.

### Default Variables

Add a list of default variables that are defined in the role's `defaults/main.yml` file.

### Other Role Variables

_No variables defined._

---

## Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be
set for other roles, or variables that are used from other roles.

---

## Installing the Role via `ansible-galaxy`

To include this role in your project using a `requirements.yml` file:

```yaml
roles:
  - name: asdf
    src: git@github.com:1000bulbs/ansible-role-asdf.git
    scm: git
    version: master
```

Then install it with:

```bash
ansible-galaxy role install -r requirements.yml
```

---

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for
users too:

```yaml
- name: My Playbook
  hosts: all
  become: true
  roles:
    - role: asdf
```

---

## Testing

This role uses [Molecule](https://molecule.readthedocs.io/) with `pytest-testinfra` for integration testing.

### Run tests locally

```bash
pip install -r requirements.txt
molecule test
```
