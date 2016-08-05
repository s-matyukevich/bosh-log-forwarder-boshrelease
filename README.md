## Bosh Log Forwarder

This bosh release contains job, that is responsible for forwarding all BOSH logs to ELK.

## Ussage

Add the following lines to all instances, for which you want to configure log forwarding.

```
  templates:
  - name: bosh-log-forwarder
    release: bosh-log-forwarder
  properties:
    elasticsearch:
      hosts: ['<host>:<port>']
      username: <username>
      password: <password>
```
