Vagrant
=========
This role installs the [Vagrant](https://www.vagrantup.com/) automation tool.


Requirements
------------
Nothing special as such but to actually use Vagrant you require some form of [virtualization](https://www.vagrantup.com/docs/getting-started/providers.html) available on the host system.

Variables
---------
``vagrant_version``: Specify the version of vagrant you want to install. By default the latest available stable version will be installed.


Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: rsjethani.vagrant }


License
-------
MIT


Author Information
------------------
Ravi Shekhar Jethani <rsjethani@gmail.com>
