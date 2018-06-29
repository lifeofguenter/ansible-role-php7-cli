[![Build Status](https://travis-ci.org/lifeofguenter/ansible-role-php7-cli.svg?branch=master)](https://travis-ci.org/lifeofguenter/ansible-role-php7-cli)

# lifeofguenter.php7-cli

This role will install PHP7 (cli) from custom built deb packages.

## Requirements

none

## Role Variables

```yaml
php7cli_default: true

php7cli_version: 7.1.19-10

php7cli_ext_apcu_version: 5.1.11-10

php7cli_ext_imagick_version: 3.4.3-10

php7cli_ext_igbinary_version: 2.0.7-10

php7cli_ext_redis_version: 3.1.6-10

php7cli_ext_iredis_version: 1.0.0-10

php7cli_ext_memcached_version: 3.0.4-10

php7cli_ext_libsodium_version: 2.0.11-10

php7cli_libsodium_version: 1.0.16-2

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
