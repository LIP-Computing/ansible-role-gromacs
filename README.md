Docker and Ansible Role: ansible-role-gromacs
=============================================

Ansible role to deploy Gromacs with CUDA support

Requirements
------------

Host machine has to have the same version of NVIDIA driver as the one
installed in by the playbook

Role Variables
--------------


Dependencies
------------

Dependent of https://github.com/LIP-Computing/ansible-role-nvidia
to previously install the nvidia driver

Example Playbook
----------------

Example of running the docker
-----------------------------

```
docker run gromacs /bin/bash -c ". /usr/local/bin/GMXRC.sh; gmx -version"
```

License
-------

GNU GPL v3

Author Information
------------------

Mario David: <mariojmdavid@gmail.com>

LIP Lisbon: http://www.lip.pt

Indigo DataCloud: https://www.indigo-datacloud.eu/
