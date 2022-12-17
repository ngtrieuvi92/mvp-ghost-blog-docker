# MVP Blogging with Ghost, Docker, Docker Compose
Quick start a blog with Ghost, Mysql, Docker & Docker-Compose running on a Ubuntu Server.
For more detail and advance config, follow the series of ghost blog development on my blog at [https://vinguyen.blog/blog-development-series-setup-mvp-ghost-blog-with-docker](https://vinguyen.blog/blog-development-series-setup-mvp-ghost-blog-with-docker/)


## Table of Contents
- [System Overview](#overview)
- [Infrastructure](#infrastructure)
- [Technolgoy Stack](#technology-stack)
- [Prerequisite](#prerequisite)
- [How to use it](#how-to-use-it)
- [License](#license)
- [References](#references)

## Overview

![ghost-deployment-diagram](https://github.com/ngtrieuvi92/mvp-ghost-blog-docker/assets/vinguyen-blog-deployment-diagram-ghost-docker.jpg)

## Infrastructure
- **Operating System** Ubuntu 22.04

- **Docker** version 20.10.21

- **Docker-compose** version 1.26.0

## Technology Stack
- Ghost blog software version 5.x
- MySQL database version 8.x

## Prerequisite
- A Ubuntu 22.04 LTS server
- A domain for your blog
- Cloudflare account linked with your domain

## How to Use this repo
1. Clone this project into the server's filesystem.
2. Create new `.env` file from `env-sample`, then edit the variable on .env if you want
```
cp env-sample .env

```
5. Run docke-compose within your server
    0. ```docker-compose up -d```  (you can remove the -d if you want to see logs, then Ctrl+C to stop all containers)
6. Go to Cloudflare and mapping your domain with server ip
7. Go to https://YOUR_DOMAIN/ghost to set up your blog.
8. Once you've made your admin account using that wizard, go back to: https://YOUR_DOMAIN/admin
9. Log in and enjoy.



## License 
MIT LICENSE

## References
+ [Ghost @ Dockerhub](https://hub.docker.com/_/ghost/)
+ [Installing Ghost locally for Dev](https://docs.ghost.org/docs/install-local)

