hetzner-ocp4-add-on-example Role
=========

This is an example add-on role for [hetzner-ocp4](https://github.com/RedHat-EMEA-SSA-Team/hetzner-ocp4)

Requirements
------------

An hetzner-ocp4 environment

Role Variables
--------------

No variables at the example

Dependencies
------------

nothing

Example hetzner-ocp4
----------------

[Install role wie CLI argument or requirements.yml](https://galaxy.ansible.com/docs/using/installing.html)
```bash
$ ansible-galaxy install git+https://github.com/RedHat-EMEA-SSA-Team/hetzner-ocp4-add-on-example.git
```

```
$ cat requirements.yml
# from GitHub
- src: https://github.com/RedHat-EMEA-SSA-Team/hetzner-ocp4-add-on-example

$ ansible-galaxy install -r requirements.yml
```

Create add-ons.yml:
```yaml
  post_install_add_ons:
    - name: hetzner-ocp4-add-on-example
      tasks_from: "post-install.yaml"
```

License
-------

Apache License 2.0

Author Information
------------------

Robert Bohne