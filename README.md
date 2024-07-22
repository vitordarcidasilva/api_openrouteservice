# API OpenRouteService

Este projeto configura e executa a API OpenRouteService com Docker.

## Estrutura de Diretórios

Antes de iniciar, certifique-se de criar os seguintes diretórios:

```bash
mkdir -p ors-docker/config ors-docker/elevation_cache ors-docke
```

## Estruções docker 

Obs: Deixei o arquivo docker-compose.yml pronto para utilizaçao dentro do Brazil, lembrando antes precisamos enviar o arquivo brazil-latest.osm.pbf para o diretório (Files)

```bash
wget https://download.geofabrik.de/south-america/brazil-latest.osm.pbf
```
```bash
sudo mv brazil-latest.osm.pbf ./Files 
```
