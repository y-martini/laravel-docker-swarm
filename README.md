```shell
git clone yuriy-martini/laravel-docker-swarm
```

```shell
docker swarm init
```

```shell
export NODE_ID=$(docker info -f '{{.Swarm.NodeID}}')
```

1. [traefik](traefik/README.md)
1. [laravel](laravel/README.md)
