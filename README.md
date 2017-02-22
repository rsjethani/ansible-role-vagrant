Vagrant
=========
This role installs the [Vagrant](https://www.vagrantup.com/) tool.


Requirements
------------
Nothing special as such but to actually use Vagrant you require some form of [virtualization](https://www.vagrantup.com/docs/getting-started/providers.html) available on the host system.

Variables
---------
``vagrant_version``: Specify the version of vagrant you want to install. If not specified then the latest stable version will be installed.

``vagrant_allow_downgrade``: Specify whether to allow downgrading current installation. If specified as ``yes`` along with vagrant_version then current installation is removed and the requested version is installed. The default value is ``no``


Example Playbook
----------------
To install latest version of vagrant:

    - hosts: servers
      roles:
         - { role: rsjethani.vagrant }

To install a specific version of vagrant:

    - hosts: servers
      roles:
         - { role: rsjethani.vagrant, vagrant_version: 1.8.5 }


License
-------
[MIT](./LICENSE)


Author Information
------------------
Ravi Shekhar Jethani <rsjethani@gmail.com>
