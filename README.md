
Para criar o arquivo `README.md` com o conteúdo ajustado, execute o comando abaixo:

```sh
echo '# API OpenRouteService

Este projeto configura e executa a API OpenRouteService com Docker.

## Estrutura de Diretórios

Antes de iniciar, certifique-se de criar os seguintes diretórios:

\`\`\`sh
mkdir -p ors-docker/config ors-docker/elevation_cache ors-docker/graphs ors-docker/files ors-docker/logs
\`\`\`

## Iniciando a Aplicação Docker

Para facilitar, deixei o arquivo \`docker-compose.yml\` pré-configurado para o Brazil, então podemos apenas executar o comando abaixo:

\`\`\`sh
docker compose up -d
\`\`\`
' > README.md
