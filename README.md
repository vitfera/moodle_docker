# Moodle Docker

Este repositório contém arquivos `docker-compose.yml` e `.env.example` para facilitar a implantação do Moodle utilizando Docker Compose com MariaDB e Redis.

## Como usar

1. Clone este repositório:
   ```bash
   git clone https://github.com/vitfera/moodle_docker.git
   ```
2. Acesse a pasta do projeto:
   ```bash
   cd moodle_docker
   ```
3. Copie o arquivo de exemplo e configure suas variáveis:
   ```bash
   cp .env.example .env
   ```
4. Edite o arquivo `.env` e ajuste as senhas e configurações conforme necessário.

5. Suba o ambiente com Docker Compose:
   ```bash
   docker compose up -d
   ```

6. Acesse o Moodle no navegador:
   - HTTP: `http://localhost`
   - HTTPS: `https://localhost`

## Serviços incluídos

- **Moodle 4.4** - Plataforma de aprendizagem
- **MariaDB 11.3** - Banco de dados
- **Redis 7.4** - Cache e gerenciamento de sessões

## Configurações importantes

Não esqueça de alterar as senhas padrão no arquivo `.env`:
- `MOODLE_ADMIN_PASSWORD`
- `MARIADB_PASSWORD`
- `MARIADB_ROOT_PASSWORD`
- `REDIS_PASSWORD`

## Sobre

Moodle é uma plataforma de aprendizagem de código aberto amplamente utilizada para educação online e gerenciamento de cursos.

---

Desenvolvido por [vitfera](https://github.com/vitfera)
