# Docker Compose Repository

## Introdução

Repositório agrupando diversos exemplos de ambientes utilizando Docker e Docker-Compose. Abaixo estão listados as opções de ambientes disponíveis:

* [Elasticsearch - Search Engine](https://www.elastic.co/guide/index.html)
* [Emby - Media Server](https://emby.media/blog.html)
* [GitLab - Source Code Management](https://docs.gitlab.com/)
* [Gogs - Git Service](https://gogs.io/docs)
* [Jenkins - Automation Server](https://www.jenkins.io/doc/book/)
* [MariaDB - Relational Database](https://mariadb.org/documentation/)
* [MongoDB - Document Database](https://docs.mongodb.com/manual/)
* [MySQL - Relational Database](https://dev.mysql.com/doc/)
* [Nextcloud - Cloud Storage Service](https://docs.nextcloud.com/)
* [ownCloud - Cloud Storage Service](https://owncloud.org/help/)
* [PostgreSQL - Relational Database](https://www.postgresql.org/docs/)
* [Redis - Data Structure Store](https://redis.io/documentation)
* [Samba - Windows Interoperability](https://www.samba.org/samba/docs/)
* [WordPress - Blog Tool](https://wordpress.org/news/)


Para utilização de todos os ambientes, é necessário que o Docker e o Docker Compose estejam instalados no Linux.


### Instalação Docker

```bash
$ sudo curl -fsSl https://get.docker.com | bash
```


### Instalação Docker Compose

```bash
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.25.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
$ sudo chmod 755 /usr/local/bin/docker-compose
```


### Clonando repositório

```bash
$ mkdir ~/Docker && cd ~/Docker
$ git clone https://github.com/RasecRapsag/docker-dompose-repository
$ cd docker-dompose-repository/
```


### Iniciando um ambiente

```bash
$ cd docker-owncloud
$ make up
```


## Comandos

Criei alguns atalhos para manipular os serviços definidos no docker-compose.

> **Nota**:
>
> Os comandos abaixo foram testados no Linux, e será necessário instalar o pacote make para funcionar.


- Para subir os serviços

```bash
$ make up
```

- Para derrubar os serviços

```bash
$ make down
```

- Para dar restart nos serviços

```bash
$ make restart
```

- Para listar os serviços

```bash
$ make ps
```

- Para verificar os logs

```bash
$ make logs
```
