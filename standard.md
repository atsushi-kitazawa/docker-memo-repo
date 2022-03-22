## standart command
```
docker images
docker ps -a
docker start <container-name>
docker stop <container-name>
docker exec -it <container-name> bash
```

## run from image
```
docker run --name <name> --rm -it -d -p 8080:8080 <image-name>:<tag>
```

## Dockerfile build
```
docker build -t <name>:<tag> .
```

## postgre command
```
docker run -d --name my_postgres -e POSTGRES_PASSWORD=mysecretpassword -e PGDATA=/var/lib/postgresql/data/pgdata -v /home/atsushi/docker/postgres:/var/lib/postgresql/data -p 15432:5432 postgres:12-alpine

# outside connection
psql -U postgres -h <host public ipaddress> -d <database-name> -p 15432
Password for user postgres: <POSTGRES_PASSWORD>
```
