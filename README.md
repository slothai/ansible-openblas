# Ansible OpenBLAS installation from source

[![Build Status](https://travis-ci.org/pavlov99/ansible-openblas.svg?branch=master)](https://travis-ci.org/pavlov99/ansible-openblas)
[![Ansible Galaxy](https://img.shields.io/ansible/role/16573.svg)](https://galaxy.ansible.com/pavlov99/openblas/)

This role installs and configures [OpenBLAS](http://www.openblas.net/) library, used for scientific computations.

### Requirements

This role requires Ansible 2.0 or higher. No other dependencies.

### Install

	ansible-galaxy install pavlov99.openblas

### Role variables

The variables that can be passed to this role and a brief description about them are as follows. (For all variables, take a look at [defaults/main.yml](defaults/main.yml))

```yaml
openblas_path: /opt/OpenBLAS
openblas_version: 0.2.19
```

### Dependencies

None

### License

MIT