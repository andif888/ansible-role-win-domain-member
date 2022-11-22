# ansible-role-win-domain-member

Ansible Role to a Windows to an AD Domain

## Table of content

- [Default Variables](#default-variables)
  - [dns_client_adapter](#dns_client_adapter)
  - [dns_client_configure](#dns_client_configure)
  - [dns_client_dns_server_ip](#dns_client_dns_server_ip)
  - [dns_domain_name](#dns_domain_name)
  - [domain_admin_password](#domain_admin_password)
  - [domain_admin_user](#domain_admin_user)
  - [hostname](#hostname)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Default Variables

### dns_client_adapter

Name of the network adapter for which DNS settings should be changed

#### Default value

```YAML
dns_client_adapter: Ethernet
```

### dns_client_configure

Re-configure DNS settings of network adapter before domain join

#### Default value

```YAML
dns_client_configure: false
```

### dns_client_dns_server_ip

DNS Server IP

#### Default value

```YAML
dns_client_dns_server_ip: 192.168.2.1
```

### dns_domain_name

AD Domain to join

#### Default value

```YAML
dns_domain_name: domain.local
```

### domain_admin_password

AD account's password with permission to join to domain

#### Default value

```YAML
domain_admin_password: vagrant
```

### domain_admin_user

AD account with permission to join to domain

#### Default value

```YAML
domain_admin_user: administrator@domain.local
```

### hostname

Name to change the hostname to

#### Default value

```YAML
hostname: '{{ inventory_hostname }}'
```



## Dependencies

None.

## License

license (GPLv2, CC-BY, etc)

## Author

andif888
