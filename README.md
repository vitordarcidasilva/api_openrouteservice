# api_openrouteservice

Vou salvar esse conteúdo em um arquivo `README.md` para você.

```sh
echo "
# API OpenRouteService

Este projeto configura e executa a API OpenRouteService com Docker.

## Estrutura de Diretórios

Antes de iniciar, certifique-se de criar os seguintes diretórios:

\`\`\`sh
mkdir -p ors-docker/config ors-docker/elevation_cache ors-docker/graphs ors-docker/files ors-docker/logs
\`\`\`

## Passos para Configuração

1. Clone este repositório:
    \`\`\`sh
    git clone https://github.com/vitordarcidasilva/api_openrouteservice.git
    cd api_openrouteservice
    \`\`\`

2. Crie e configure os diretórios necessários:
    \`\`\`sh
    mkdir -p ors-docker/config ors-docker/elevation_cache ors-docker/graphs ors-docker/files ors-docker/logs
    \`\`\`

## Executando o Docker

Para executar a API OpenRouteService usando Docker, siga as instruções abaixo.

### Build da Imagem Docker

\`\`\`sh
docker build -t ors-image .
\`\`\`

### Executando o Container Docker

\`\`\`sh
docker run -d -p 8080:8080 -v \$(pwd)/ors-docker/config:/ors-core/openrouteservice/src/main/resources/ors/configs -v \$(pwd)/ors-docker/elevation_cache:/ors-core/data/elevation_cache -v \$(pwd)/ors-docker/graphs:/ors-core/data/graphs -v \$(pwd)/ors-docker/files:/ors-core/data/files -v \$(pwd)/ors-docker/logs:/ors-core/log ors-image
\`\`\`

### Acessando a API

Após iniciar o container, a API estará disponível em \`http://localhost:8080\`.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
" > README.md
