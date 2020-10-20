### Container para Rodar PHP e Firebird

#### Passo 1 - Construir a imagem 

```bash
docker container prune -f

docker-compose build --no-cache --pull

ou 

docker-compose up --build --force-recreate
```

#### Execututando o container

```bash
docker-compose up
```

#### Parando o container

```bash
docker-compose down
```

#### Limpeza 

# setup.sh

# Start "stage" service
docker-compose up stage

# Commit changes to an image named "stage"
docker commit $(docker-compose ps -q stage) stage

# Start setup service off of stage image
docker-compose up setup



docker-compose -f docker-compose.yml down
docker container prune -f
docker-compose -f docker-compose.yml up --build


