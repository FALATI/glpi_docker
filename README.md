# GLPI com Docker Compose

Este repositório contém os arquivos necessários para executar o GLPI.

## Pré-requisitos

- [**Docker Engine**](https://docs.docker.com/engine/install/)
- [**Docker Compose**](https://docs.docker.com/compose/install/)

## Inicializando a Stack

```bash
docker compose up --detach
```

## Acessando e configurando o GLPI

Observe que no [`docker-compose.yaml`](docker-compose.yaml) o host do GLPI é `glpi-127-0-0-1.nip.io`. Mude este host no compose para o de sua preferência. Ajuste o seu DNS.
> Os hosts padrões estão utilizando o serviço https://nip.io/ para uso local.

Acessando o GLPI: http://glpi-127-0-0-1.nip.io/

```bash
host: mariadb
usuario: glpi
senha: glpi
```

## Usuário e senha padrão para acesso ao GLPI

```bash
Usuário: glpi
Senha: glpi
```

## Acessando o dashboard do Traefik
```
URL: http://traefik-127-0-0-1.nip.io/
Usuário: admin
Senha: password
```
