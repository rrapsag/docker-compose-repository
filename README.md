# Docker Compose Repository

## Introdução

Repositório agrupando diversos exemplos de ambientes utilizando Docker e Docker-Compose. Abaixo estão listados as opções de ambientes disponíveis:

* [Elasticsearch - Search Engine](https://www.elastic.co/guide/index.html)
* [Emby - Media Server](https://emby.media/blog.html)
* [GitLab - Source Code Management](https://docs.gitlab.com/)
* [Gogs - Git Service](https://gogs.io/docs)
* [Jellyfin - Media Server](https://jellyfin.org/docs/)
* [Jenkins - Automation Server](https://www.jenkins.io/doc/book/)
* [MailHog - Email Testing Tool](https://github.com/mailhog/MailHog)
* [MariaDB - Relational Database](https://mariadb.org/documentation/)
* [MongoDB - Document Database](https://docs.mongodb.com/manual/)
* [MySQL - Relational Database](https://dev.mysql.com/doc/)
* [Nextcloud - Cloud Storage Service](https://docs.nextcloud.com/)
* [ownCloud - Cloud Storage Service](https://owncloud.org/help/)
* [Pi-hole - Network-wide Protection](https://docs.pi-hole.net/)
* [Portainer - Container Manager](https://documentation.portainer.io/)
* [PostgreSQL - Relational Database](https://www.postgresql.org/docs/)
* [Redis - Data Structure Store](https://redis.io/documentation)
* [Samba - Windows Interoperability](https://www.samba.org/samba/docs/)
* [SQL Server Linux - Relational Database](https://docs.microsoft.com/pt-br/sql/linux)
* [WordPress - Blog Tool](https://wordpress.org/news/)
* [Homer - Personal Dashboard](https://github.com/bastienwirtz/homer/)
* [Unbound - DNS Resolver](https://www.nlnetlabs.nl/projects/unbound/about/)
* [Navidrome - Music and Streamer Server](https://www.navidrome.org/docs/)
* [Windows 2000 - Operating System](https://github.com/hectorm/docker-qemu-win2000)
* [Apache Guacamole - Remote Desktop Gateway](https://guacamole.incubator.apache.org/doc/gug/)
* [Whoogle - Search Engine](https://github.com/benbusby/whoogle-search)
* [File Browser - File Manager](https://filebrowser.org/)
* [JDownloader - Download Management Tool](https://jdownloader.org/)
* [Uptime Kuma - Monitoring Tool](https://github.com/louislam/uptime-kuma/wiki)
* [Watchtower - Container Image Update](https://containrrr.dev/watchtower/)
* [Snippet Box - Simple Code Snippet Organizer](https://github.com/pawelmalak/snippet-box)
* [PhotoPrism - Photo App](https://www.photoprism.app)
* [Heimdall - Application Dashboard](https://heimdall.site/)
* [2FAuth - Two-Factor Authentication](https://2fauth.app/)
* [Audiobookshelf - Audiobook and Podcast Server](https://www.audiobookshelf.org/)
* [Metube - Youtube Downloader](https://github.com/alexta69/metube)
* [Calibre - E-book Management](https://calibre-ebook.com/)


Para utilização de todos os ambientes, é necessário que o Docker e o Docker Compose estejam instalados no Linux.


### Instalação Docker

```bash
$ sudo curl -fsSl https://get.docker.com | bash
```


### Instalação Docker Compose

```bash
$ sudo curl -L "https://github.com/docker/compose/releases/download/v2.32.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
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
