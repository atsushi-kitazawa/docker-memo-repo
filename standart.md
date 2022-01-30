## standart command
```
docker ps -a
docker start <container-name>
docker stop <container-name>
docker exec -it <container-name> bash
```

## postgre command
```
docker run -d --name my_postgres -e POSTGRES_PASSWORD=mysecretpassword -e PGDATA=/var/lib/postgresql/data/pgdata -v /home/atsushi/docker/postgres:/var/lib/postgresql/data -p 15432:5432 postgres:12-alpine

# outside connection
psql -U postgres -h <host public ipaddress> -d <database-name> -p 15432
Password for user postgres: <POSTGRES_PASSWORD>
```
