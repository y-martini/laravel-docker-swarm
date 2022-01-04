```shell
docker network create --driver=overlay traefik-public
```

```shell
docker node update --label-add traefik-public.traefik-public-certificates=true $NODE_ID
```

```shell
cp example.env .env
```

```shell
vim .env
```

```shell
source .env
```

```shell
export HASHED_PASSWORD=$(openssl passwd -apr1 $PASSWORD)
```

```shell
docker stack deploy -c traefik.yml traefik
```
