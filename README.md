isset.unattended-upgrades [![pipeline status](https://gitlab.isset.nl/operations/isset.unattended-upgrades/badges/master/pipeline.svg)](https://gitlab.isset.nl/operations/isset.unattended-upgrades/commits/master)
=========

_Installs unattended-upgrades._

Requirements
------------

Ansible 2.5 or above is highly recommended.

Role Variables
--------------

    isset_unattended_upgrades_enabled: True
    isset_unattended_upgrades_state: installed
    isset_unattended_upgrades_unattended_upgrade: 1
    isset_unattended_upgrades_autoclean_interval: 7
    isset_unattended_upgrades_mailto: root
    isset_unattended_upgrades_remove_old_kernels: true
    isset_unattended_upgrades_remove_unused_dependencies: true
    isset_unattended_upgrades_automatic_reboot: true
    isset_unattended_upgrades_automatic_reboot_time: "02:00"

Dependencies
------------

    isset.package

Example Playbook
----------------

    - hosts: all
      become: yes
      roles:
        - role: isset.unattended-upgrades

License
-------

MIT

Author Information
------------------

Gerben Geijteman <gerben@isset.nl>
