## The Docker Compose File

The `docker-compose.yml` file defines 
how we run all of our bots.

These are a compilation of docker-compose 
files found in individual bot repos.

To build the containers in the pod:

```
docker-compose build
```

To rebuild from scratch without using any cached data:

```
docker-compose build --no-cache
```

To bring the entire container pod up:

```
docker-compose up          # interactive
docker-compose up -d       # detached
docker-compose up --build  # build before running
```

To stop the docker bot pod, use the stop
or down commands.

Stop the container but keep the volumes/networks:;

```
docker-compose stop
```

stop the container and remove infrastructure:

```
docker-compose down
```


## Testing Out Individual Bots

To test out the containers for each individual bot,
you can just cd into that bot's directory and 
run the same commands as above. That will build/start
a container that runs only that one bot.

