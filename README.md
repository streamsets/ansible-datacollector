streamsets.datacollector
=========

[StreamSets Data Collector](http://streamsets.com) - An open source data collector.

Requirements
------------

The role currently expects that you already have a JRE installed on the target
system. Oracle Java 8 is recommended.

Role Variables
--------------

Defaults are provided for the most commonly changed parameters in
`defaults/main.yml`. For a full list of available variables please review the
templates directly.

Dependencies
------------

None.

Example Playbook
----------------

Basic usage only requires specifying the role. To run multiple instances on a
single machine you can specify custom values for `sdc_instance` and `http_port`

    - hosts: datacollectors
      roles:
         - { role: streamsets.datacollector, sdc_instance: 'datacollector_1', http_port: 18630 }
         - { role: streamsets.datacollector, sdc_instance: 'datacollector_2', http_port: 18640 }

License
-------

[Apache License, Version 2.0](https://tldrlegal.com/license/apache-license-2.0-(apache-2.0))

Author Information
------------------

- [Adam Kunicki](https://adamkunicki.com/) | [e-mail](mailto:adam@streamsets.com) | [Twitter](https://twitter.com/ramblingpolak)
