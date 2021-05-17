Ansible Role: NGINX(pkg)
================================================================================
Install and configure NGINX as an HTTP Server

- Install NGINX 1.18.* using yum at CentOS 7
- Configure files in /etc/nginx
- Open tcp/80 and tcp/443

Requirements
--------------------------------------------------------------------------------
None

Role Variables
--------------------------------------------------------------------------------
The following variables are defined in defaults/main.yml file.

```yaml
nginx:
  enabled: true
  started: true
  serverroot: "/etc/nginx"
  configroot: "/etc/nginx/conf.d"
  workingdir: "/usr/local/src"
```

Dependencies
--------------------------------------------------------------------------------
None

Example Playbook
--------------------------------------------------------------------------------
```yaml
- hosts: servers
  roles:
     - { role: azumakuniyuki.ar-nginx-pkg }
```

License
--------------------------------------------------------------------------------
BSD

Author Information
--------------------------------------------------------------------------------
[azumakuniyuki](https://nyaan.jp)

