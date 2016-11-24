# Docker for celery flower

### Description

This is a [flower](https://github.com/mher/flower) docker, and use redis for broker

### Run

Use the command below:

```bash
docker run -d --name=flower -p 5555:5555 playniuniu/flower
```

The default redis url is **redis://redis:6379/0**, if you try to use other redis url

```bash
docker run -d --name=flower -p 5555:5555 -e REDIS_BROKER="YOUR_REDIS_URL" playniuniu/flower
```