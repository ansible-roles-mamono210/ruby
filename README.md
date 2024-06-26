[![CircleCI](https://circleci.com/gh/ansible-roles-mamono210/ruby/tree/main.svg?style=svg)](https://circleci.com/gh/ansible-roles-mamono210/ruby/tree/main)

Role Description
=========

Installs [Ruby](https://www.ruby-lang.org) from source for CentOS Stream 9.

Requirements
------------

None

Role Variables
--------------

| Name | Description | Default value |
|------|------|-------|
| workspace | The location where temporary files will be downloaded in preparation for Ruby installation. | /tmp |
| ruby_download_url | The URL from which Ruby will be downloaded | http://cache.ruby-lang.org/pub/ruby/3.0/ruby-3.0.0.tar.gz | |
| ruby_version | The version of ruby that will be installed | 3.0.0 |
| ruby_source_configure_command | The configure command that will be run | ./configure --enable-shared |

Dependencies
------------

None

Example Playbook
----------------

```YAML
---
- hosts: all
  become: true
  roles:
    - ruby
```

License
-------

BSD
