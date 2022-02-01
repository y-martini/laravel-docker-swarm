```shell
docker node update --label-add db.mysql-data=true $NODE_ID
```

```shell
cp example.env .env
```

```shell
vim .env
```

```shell
env $(cat .env | grep ^[A-Z] | xargs) \
docker stack deploy -c db.yml db
```
