## Build and start

```sh
docker compose build
docker images
docker compose up -d
```

`build` is not really neccessary `docker compose up -d` will build if still not builded previously.

## Get IP address

```sh
ip addr show  # 3: eth1 / inet 192.168.56.38
```

Open in the browser: `http://192.168.56.38/`
username: admin_vp
pw: admin_vp

## Push to DockerHub

```sh
docker login
docker images
docker push lendoo73/vprofileapp
```

## Stop containers

```sh
docker compose ps

docker compose stop
docker compose rm

# or
docker compose down # stop then remove
```

```sh
docker system prune -a
```