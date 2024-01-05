# docker-db-postgres

## it's a simple config for docker postgreSQL

Folder "postgres_data" is't a folder which cantains data from Docker volume, it's kind of share folder betwin container and local

## Get started
When you init your DB config with username and password, you create your container with
```docker compose up``` or ```docker-compose up```

You can go inside your container in order to see if it's running
```docker exec -it <containerName> sh```

Inside your container check if your config running good with your credentials
```psql -h localhost -p 5432 -U <myuser> -d <mydatabase>```
