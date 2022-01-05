```shell
git clone https://github.com/yuriy-martini/laravel-docker-swarm
```

```shell
docker swarm init
```

```shell
docker swarm init --advertise-addr x.x.x.x
```

```shell
export NODE_ID=$(docker info -f '{{.Swarm.NodeID}}')
```

1. [traefik](traefik/README.md)
1. [laravel](laravel/README.md)
