### Container para Rodar PHP e Firebird

#### Passo 1 - Construir a imagem 
```
docker container prune -f

docker-compose -f docker-compose-v1.yaml build --no-cache --pull
```

#### Execututando o container
```
docker-compose -f docker-compose-v1.yaml up
```

#### Parando o container
```
docker-compose -f docker-compose-v1.yaml down
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


