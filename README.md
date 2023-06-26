# Webarchitects GeoIP Update Ansible role

An Ansible role to download and install the latest [GeoIP
update](https://github.com/maxmind/geoipupdate) from
[GitHub](https://github.com/maxmind/geoipupdate/releases/latest) as a `.deb`.

This role requires a [license key](https://www.maxmind.com/en/my_license_key).

See also the [MaxMind DB Apache Module
role](https://git.coop/webarch/modmaxminddb).

## Role variables

Set `geoipupdate` to `true` for the tasks in this role to be run.

Documentation for the [defaults/main.yml](defaults/main.yml) variables follow,
this documentation has been generated from the
[meta/argument_specs.yml](meta/argument_specs.yml).

### Entrypoint: main

The main entry point for the geoipupdate role.

|Option|Description|Type|Required|
|---|---|---|---|
| geoipupdate | Run the tasks in this role. | bool | yes |
| geoipupdate_account_id | Account ID from MaxMind. | str | yes |
| geoipupdate_license_key | License key from MaxMind. | str | yes |
| geoipupdate_edition_ids | A list of MaxMind database editions. | list of 'str' | yes |

## Repository

The primary URL of this repo is
[`https://git.coop/webarch/geoipupdate`](https://git.coop/webarch/geoipupdate)
however it is also [mirrored to
GitHub](https://github.com/webarch-coop/ansible-role-geoipupdate) and
[available via Ansible
Galaxy](https://galaxy.ansible.com/chriscroome/geoipupdate).

See the [GitLab releases page](https://git.coop/webarch/geoipupdate/-/releases)
for details regarding each version, *please use a specific version* since the
master branch is used for development.

## Copyright

Copyright 2019-2023 Chris Croome,
&lt;[chris@webarchitects.co.uk](mailto:chris@webarchitects.co.uk)&gt;.

This role is released under [the same terms as Ansible
itself](https://github.com/ansible/ansible/blob/devel/COPYING), the [GNU
GPLv3](LICENSE).
