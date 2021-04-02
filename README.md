Role Name
=========

This role is used for installing checking if pipenv environment is initialized, and installing dependencies if it is not. Optionally you can force a rebuild of the env, by passing the variable `force: true` to the role. Also, you can pass in extra arguments to pipenv with the `pipenv_extra_args` and `pipenv_dev_extra_args` ( for the dev install ).

Requirements
------------

Python3 and pip3 need to be installed on the remote system. I handle the pathing for python executables with `python_path`.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

N/a

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: elreydetoda.pipenv, dev_env: true, project_root: '/home/vagrant/' }

License
-------

LGPL

Author Information
------------------

<https://elrey.casa/blog>
