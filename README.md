Vector
=========

This role can install Vector on Centos and Ubuntu

Role Variables
--------------

| vars | description |
|------|-------------|
| vector_version | Version of Vector (default 0.21.0) |
| vector_config_dir | Path to the directory with vector files |
| clickhouse_server | IP address clickhouse server (default 127.0.0.1) |
| clickhouse_port | Port clickhouse server (default 8123) |

Example Playbook
----------------

```yaml
- name: Install Vector
  hosts: vector
  tags:
    - vector
  roles:
    - vector
  vars:
    vector_version: "0.21.0"
    vector_config_dir: /var/lib/vector
    clickhouse_server: "127.0.0.1"
    clickhouse_port: "8123"
```

License
-------

MIT

Author Information
------------------

Pavel Chashkov
