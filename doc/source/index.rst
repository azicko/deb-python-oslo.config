oslo.config
===========

An OpenStack library for parsing configuration options from the command
line and configuration files.

Contents
--------

.. toctree::
   :maxdepth: 1

   api/autoindex

Release Notes
=============

1.2.0a3
-------

* 1176817_: Fix the priority of CLI args vs config file values
* 1123043_: New 'choices' param to StrOpt constructor
* cfg-reload-config-files_: Add new ConfigOpts.reload_config_files() method
* 1194742_: Fix regression which meant we weren't registering our namespace package
* 1185959_: Make --help output order alphabetical
* More progress on python3 support
* Fix obscure cache clearing race condition
* Move from tools/pip-requires to requirements.txt
* Include missing .testr.conf in dist tarball

.. _1176817: https://bugs.launchpad.net/oslo/+bug/1176817
.. _1123043: https://bugs.launchpad.net/oslo/+bug/1123043
.. _cfg-reload-config-files: https://blueprints.launchpad.net/oslo/+spec/cfg-reload-config-files
.. _1194742: https://bugs.launchpad.net/oslo/+bug/1194742
.. _1185959: https://bugs.launchpad.net/oslo/+bug/1185959

1.2.0a2
-------

* Fix MultiConfigParser API breakage in 1.2.0a1

1.2.0a1
-------

* Solid progress has been made adding Python 3 support.
* cfg-lowercase-groups_: uppercase section names in config files are now normalized to lowercase.
* Support has been added for dictionary style options with the ``DictOpt`` class.
* Multiple deprecated option names per option are now supported via the ``deprecated_opts`` argument.
* The package build process now uses pbr_.
* The package tests are now run using testr_.
* The package coding style checks are now performed using hacking_.

.. _cfg-lowercase-groups: https://blueprints.launchpad.net/oslo/+spec/cfg-lowercase-groups
.. _pbr: http://docs.openstack.org/developer/pbr/
.. _testr: https://wiki.openstack.org/wiki/Testr
.. _hacking: https://pypi.python.org/pypi/hacking

1.1.1
-----

* 1160922_: Fix set_defaults() to handle multiple arguments
* 1175096_: Fix the title argument to ``OptGroup``

.. _1160922: https://bugs.launchpad.net/oslo/+bug/1160922
.. _1175096: https://bugs.launchpad.net/oslo/+bug/1175096

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

