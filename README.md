# GLUSTER FS
Network File System


## Installation


Gluster Server
```bash
    ansible-playbook -i inventory/hosts  01_gluster_server.yml
```

Gluster Client

```bash
    ansible-playbook -i inventory/hosts  02_gluster_client.yml
```

Check status
` gluster peer status `


Probe gluster connection
` gluster peer probe $ANOTHER_GLUSTER_SERVER_HOST`