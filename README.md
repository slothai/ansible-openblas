# Ansible OpenBLAS installation from source

[![Build Status](https://travis-ci.org/slothai/ansible-openblas.svg?branch=master)](https://travis-ci.org/slothai/ansible-openblas)
[![Ansible Galaxy](https://img.shields.io/ansible/role/16762.svg)](https://galaxy.ansible.com/slothai/openblas/)

This role installs and configures [OpenBLAS](http://www.openblas.net/) library, used for scientific computations.

### Requirements

This role requires Ansible 2.0 or higher. No other dependencies.

### Install

    ansible-galaxy install slothai.openblas

### Role variables

The variables that can be passed to this role and a brief description about them are as follows. (For all variables, take a look at [defaults/main.yml](defaults/main.yml))

```yaml
openblas_path: /opt/OpenBLAS
openblas_version: 0.2.19
openblas_no_affinity: 1  # NO_AFFINITY=1 flag
# Uncomment line below to set USE_OPENMP. Its enabled for multi-core systems.
# openblas_use_openmp: 1
```

It uses `{{ansible_processor_vcpus}}` threads by default and enables `USE_OPENMP=1` for 2+ cpus.

### Dependencies

None

### License

MIT
