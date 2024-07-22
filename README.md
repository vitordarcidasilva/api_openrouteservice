# API OpenRouteService

Este projeto configura e executa a API OpenRouteService com Docker.

## Estrutura de Diretórios

Antes de iniciar, certifique-se de criar os seguintes diretórios:

```sh
mkdir -p ors-docker/config ors-docker/elevation_cache ors-docker/graphs ors-docker/files ors-docker/logs

#Para facilitar deixei o arquivo docker-compose.yml pré configurado para o Brazil então podemos apenas executar o comando abaixo.

'''sh docker compose up -d
