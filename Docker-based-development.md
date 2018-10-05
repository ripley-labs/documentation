# Docker COMPOSE commands

## Run a docker compose stack using a custom docker-compose.yml file

Go to your project root directory and then:

```
docker-compose -f <your-custom-docker-compose-file> up -d --build --force-recreate; docker-compose logs -f
```

To close logs, just ctrl-c (your stack will continue running in background)

## Remove every container created by a docker-compose.yml

Go to your project root directory and then:

```
docker-compose -f <your-custom-docker-compose-file> down
```

## Run a command inside a temporal container based on a service defined in a custom docker-compose.yml file


```
docker-compose run --rm -w <working directory inside container> <service-name> <custom command>
```

### Practical examples:

Installing node modules dependencies through a docker container:
```
docker-compose -f docker-compose.yml run --rm -w /app node npm install --verbose
```

Get dependencies of python environment and save to requirements.txt
```
docker-compose -f docker-compose.yml run --rm -w /app python pip3 freeze > requirements.txt
```
