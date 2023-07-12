# Retrieving and sending Cisco IOS configs without Jinja2 templates

Repository for the blog post: [**TODO**].

## Run

Provide a config file as an Ansible extra variable with the command line using the --extra-vars (or -e) argument.

### 1. Parse

Parse a Cisco IOS configuration.

```
$ ansible-navigator run parse.yml -e config=config.cfg
```

### 2. Generate aggregated data

Aggregate data and try to run it through a Resource Module. [**Work In Progress**]

```
$ ansible-navigator run generate.yml
```

## Links

- [ansible.utils.consolidate](https://github.com/ansible-collections/ansible.utils/blob/main/docs/ansible.utils.consolidate_filter.rst#ansibleutilsconsolidate)
- [ios_route_maps doesn't parse full configuration files](https://github.com/ansible-collections/cisco.ios/issues/884)
- [Add support for Network Address Translation (NAT)](https://github.com/ansible-collections/cisco.ios/issues/885)
- [Add parsed and rendered states to ios_vrf](https://github.com/ansible-collections/cisco.ios/issues/886)
- [Add parsed and rendered states to ios_system](https://github.com/ansible-collections/cisco.ios/issues/887)
- [ios_vlans tries to connect to device for parsed](https://github.com/ansible-collections/cisco.ios/issues/888)
