lxd_network
==========

A module for managing the networks configuration in lxd.<br/>
It is heavily based on the lxd_profile module by [Hiroaki Nakamura](https://github.com/hnakamur)

Requirements
------------

  - lxd > 2.1X (network feature)

Example Task
------------

    - name: Create a network
      lxd_network:
        name: lxdbr0
        description: Default bridge
        config:
          ipv4.address: 172.29.0.1/24
          ipv4.nat: "true"
          ipv6.address: none

Additional informations
=======================

A pull request has been [created](https://github.com/ansible/ansible/pull/31428)

License
-------

GNU GPLv3

Author Information
------------------

Sofiane MEDJKOUNE
