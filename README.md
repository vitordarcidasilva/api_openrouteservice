# API OpenRouteService

Este projeto configura e executa a API OpenRouteService com Docker.

## Estrutura de Diretórios

Antes de iniciar, certifique-se de criar os seguintes diretórios:

```bash
mkdir -p ors-docker/config ors-docker/elevation_cache ors-docker/graphs ors-docker/files ors-docker/logs
```

## Estruções docker 

Obs: Deixei o arquivo docker-compose.yml pronto para utilizaçao dentro do Brazil, lembrando antes precisamos enviar o arquivo brazil-latest.osm.pbf para o diretório (Files)

```bash
wget https://download.geofabrik.de/south-america/brazil-latest.osm.pbf
```
```bash
sudo mv brazil-latest.osm.pbf ./files
```

## Inciando a aplicação 

```bash
docker-compose up -d
```
## Verificando status da api

```bash
http://localhost:8080/ors/v2/status
```

## Verificando logs docker

```bash
docker compose logs -tf
```

## Testando a APi

obs: Precisamos colocar as latitude e longitude invertidas.

```bash
http://localhost:8080/ors/v2/directions/driving-car?&start=-46.5258548,-23.4318942,&end=-46.525788,-23.452317)
```



