[![Build Status](https://travis-ci.org/lifeofguenter/ansible-role-php7-cli.svg?branch=master)](https://travis-ci.org/lifeofguenter/ansible-role-php7-cli)

# lifeofguenter.php7-cli

This role will install PHP7.1 (cli) from custom built deb packages.

_Please note: this is simply meant as a interim to have PHP7.1 on the flavours:
debian jessie/stretch + ubuntu trusty/xenial. The packages are compiled from
source with no additional patches, so production ready, but please keep updated
and scrutinise it before using._

_Deb-packages are pre-generated with `checkinstall` just to avoid compiling from
scratch during each ansible run._

## Requirements

none

## Role Variables

```yaml
php7cli_default: true

php7cli_version: 7.1.26-22

php7cli_ext_apcu_version: 5.1.16-22

php7cli_ext_apcu_bc_version: 1.0.4-22

php7cli_ext_imagick_version: 3.4.3-22

php7cli_ext_igbinary_version: 2.0.8-22

php7cli_ext_redis_version: 3.1.6-22

php7cli_ext_iredis_version: 1.0.0-22

php7cli_ext_memcached_version: 3.0.4-22

php7cli_ext_libsodium_version: 2.0.20-22

php7cli_ext_geoip_version: 1.1.1-22

php7cli_ext_mailparse_version: 3.0.2-22

php7cli_ext_gnupg_version: 1.4.0-22

php7cli_libsodium_version: 1.0.16-3

php7cli_conf_apc_shm_size: 256M
```

## Dependencies

none

## Example Playbook

```yaml

- hosts: servers
  roles:
    - { role: lifeofguenter.php7-cli }
```

## License

Licensed under the MIT License. See the [LICENSE file](LICENSE) for details.

## Author Information

[Gunter Grodotzki](https://lifeofguenter.de)
