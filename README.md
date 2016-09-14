JBoss Forge
=========

This role install JBoss Forge command line tool and makes the tool available throught the user path

Requirements
------------

JDK8+

Role Variables
--------------

- __forge_version__: version of product. _3.3.0.Final_ by default
- __forge_user_to_bashrc__: user to insert tool path in bashrc
- __forge_install_dir__: /usr/local/jboss by default.

Dependencies
------------

Some role that installs a JDK8.

Example Playbook
----------------



    - hosts: servers
	  vars:
	     - forge_user_to_bashrc: "vagrant"
      roles:
         - { role: dpalomar.jboss-forge }

License
-------

MIT / BSD

Author Information
------------------

Role created by David Palomar
