```shell
docker node update --label-add laravel.app-data=true $NODE_ID
```

```shell
docker node update --label-add laravel.queue-worker-data=true $NODE_ID
```

```shell
docker node update --label-add laravel.schedule-runner-data=true $NODE_ID
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
docker stack deploy -c laravel.yml laravel
```
