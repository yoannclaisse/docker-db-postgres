# docker-db-postgres

## it's a simple config for docker postgreSQL

Folder "postgres_data" is't a folder which cantains data from Docker volume, it's kind of share folder betwin container and local

## Get started with postgres
When you init your DB config with username and password, you create your container with
```docker compose up``` or ```docker-compose up```

You can go inside your container in order to see if it's running
```docker exec -it <containerName> sh```

Inside your container check if your config running good with your credentials
```psql -h localhost -p 5432 -U <myuser> -d <mydatabase>```

## Get started with pgadmin4
In order to see your work with postgres I add pgadmin4 here => http://localhost:5050 use your credentials that you use inside docker-compose.yaml

Add a new PostgreSQL server to pgAdmin using the following information:

Server Name: Choose a meaningful name
Host: postgres
Port: 5432
Database Name, Username, Password: Use the values you defined in the docker-compose.yml file

