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
export HASHED_PASSWORD=$(openssl passwd -apr1)
```

```shell
env $(cat .env | grep ^[A-Z] | xargs) \
docker stack deploy -c traefik.yml traefik
```
