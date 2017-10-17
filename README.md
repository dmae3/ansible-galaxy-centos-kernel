Kernel setting role
=========

Kernel setting ansible galaxy role.

Requirements
------------

None

Role Variables
--------------

* kernel_parameter_file_path  
kernel parameter config file path.  
default:  
`/etc/sysctl.d/10-system.conf`

* kernel_parameters  
kernel parameter key and value.  
e.g.  

```yml
kernel_parameters:
  - name: kernel.panic
    value: 10
  - name: fs.file-max
    value: 150298
```

Dependencies
------------

None

Example Playbook
----------------

```yml
---
- hosts: all
  become: true
  roles:
    - { role: galaxy-centos-kernel }
```

License
-------

BSD

Author Information
------------------

[Daisuke Maeda](https://github.com/dmae3 "Daisuke Maeda")
