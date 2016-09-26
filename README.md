# Python Nailgun Client

[![N|Solid](https://static.fuel-infra.org/fuel/logo/fuel-logo-400x180.png)](https://wiki.openstack.org/wiki/Fuel)

This a tool for create and deploy Fuel Clusters from prepared config files.

Supported versions:
  - 9.1
  - 9.0
  - 8.0
  - 7.0
  - 6.1
  - 6.0.1
  - 5.1.2

The main part was based on [mos-components-ci][mcc] framework and modified for last Fuel releases.

### Installation

Nailgun Client requires [Keytone Client](https://github.com/openstack/python-keystoneclient) to run.

Create a python virualenv and install the dependencies.

```sh
$ virtualenv .venv
$ source .venv/bin/activate
$ pip install -r requirements.txt
```

### Prepare configuration file

Sample configuration file can be found here:

* [sample.config.ini] [sample_config]

More details coming soon.

### Run

For start tool to create, configuring and deploy Fuel Environment you should be execute this command:
```sh
$ nailgun.py <config_file_name> <fuel_ui_ip>:<fuel_ui_port> <virtual_servers_count> <baremetal_servers_count>
```

For example:
```sh
$ nailgun.py config.ini 172.18.173.5:58205 5 0
```

### Todos

 - Prepare manuals
 - Prepare python egg package
 - Rewrite CLI client

License
----

[Apache v2.0](https://github.com/molecul/fuel-nailgun_client_deployment/blob/master/LICENSE)



   [mcc]: <https://github.com/Mirantis/mos-components-ci>
   [fuel]: <https://wiki.openstack.org/wiki/Fuel>
   [sample_config]: <https://github.com/molecul/fuel-nailgun_client_deployment/tree/master/sample.config.ini>

