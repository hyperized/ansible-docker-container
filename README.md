# ansible-docker-container
An Ansible Docker container role for Ubuntu 14.04 with Upstart scripts

## Prerequisites

This role assumes you run a docker daemon on Ubuntu 14.04

## Usage

Include the folder in your roles directory. You can edit the configuration in, for example, your group_vars, like this:

```
docker_containers:
   - name: redis
   - name: mystuff
     image: myrepository/mydocker:myversion
     published_ports: 80:80
     env:
       HELLO: WORLD
```

## Author

Gerben Geijteman <gerben@hyperized.net>

## License

MIT