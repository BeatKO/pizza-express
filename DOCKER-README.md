# Running application in Docker container

Run:

```
docker-compose up -d
```

or:

```
docker build -t pizza:latest .
docker run --name redis-host -d -p 6379:6379 redis
docker run --name pizza-app -d -p 8081:8081 --link=redis-host pizza:latest
```
