# This is a simple news admin panel
## I use docker and docker compose

# Installation
# STEP 1 Open terminal in current directory and insert this command 
```make build```
### This command create docker image and docker containers and run project

# STEP 2 Enter in phpmyadmin in address: http://localhost:777 and create database with name admin

# STEP 3 Port for connection database: 6033 Look at docker-compose.yml
```localhost:6033```

# STEP 4 Create tables with name news and author
```
CREATE TABLE news(
    id SERIAL,
    title TEXT,
    content TEXT,
    author VARCHAR(255)
);
```

```
CREATE TABLE author (
   id SERIAL,
   name varchar(255) DEFAULT NULL
);
```

# STEP 5  Look at in browser link: http://localhost:83


# HELP COMMANDS

## Command give you write log.txt
```chmod ugo+rwx log.txt```

# Enter internal run docker container
```docker exec -it php-simple-admin bash```
