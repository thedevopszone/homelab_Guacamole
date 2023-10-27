# Guacamole

## Links

- https://github.com/oznu/docker-guacamole
- https://guacamole.apache.org/doc/gug/guacamole-docker.html


## Docker

vi docker-compose.yml
```
version: "2"
services:
  guacamole:
    image: oznu/guacamole
    container_name: guacamole
    volumes:
      - postgres:/config
    ports:
      - 8080:8080
volumes:
  postgres:
    driver: local
```


