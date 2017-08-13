# PHPDF Site - Docker

[Versão em Português](./README.md)

Now it is possible to have the site have the entire Stack of the new PHPDF website directly on your machine, enabling follow-up, sending of suggestions and improvements.

### About

The reverse proxy solutions for this repository have been provided by repo [devbrotherhood/docker-reverse-proxy](https://github.com/devbrotherhood/docker-reverse-proxy) and are used to bind multiple domains to specific port applications for Docker, allowing multiple containers to run on different ports, but responding to a default port such as 80.

### How to use

In this solution, we use the docker-compose tool from Docker.

Let's take the steps:

- Add your host to `/etc/hosts`
- Duplicate the `docker-compose.yml_sample` and `./conf/my_proxy.conf_sample` files respectively to `docker-compose.yml` and `./conf/my_proxy.conf`, adjusting according to your needs.
- Run the command below so that docker raises the entire stack of your application:

```
     docker-compose up
```

### References

- https://github.com/devbrotherhood/docker-reverse-proxy