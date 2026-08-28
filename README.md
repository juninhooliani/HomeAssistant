# Projeto Home Assistant + OpenWiki

Este repositório contém a infraestrutura em Docker e a base de conhecimento (OpenWiki) para gerenciamento do Home Assistant.

## Como Executar o Home Assistant

1. Certifique-se de ter o **Docker Desktop** instalado e rodando.
2. Abra o terminal nesta pasta (`d:\Google Drive\Pessoal\Projetos\HomeAssitant`) e execute:

```bash
docker compose up -d
```

3. Acesse o Home Assistant no navegador pelo endereço:
   [http://localhost:8123](http://localhost:8123)

## Estrutura do Projeto
- `docker-compose.yml`: Configuração do contêiner Docker.
- `config/`: Configurações do Home Assistant.
- `openwiki/`: Base de conhecimento para documentação e contexto de IA (LangChain OpenWiki).
- `AGENTS.md`: Arquivo de instruções para agentes de inteligência artificial.
