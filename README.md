# Symfony Docker Starter

> An Symfony starter kit featuring 
[Symfony](https://symfony.com/) and 
[Docker](https://www.docker.com/) 
([PHP], 
[MySQL], 
[Memcached],
and [Nginx])

This seed repo serves as an Symfony starter for anyone looking to get up and running with Symfony and PHP fast. Using Docker for building our environment.

* Ready to go development environment using Docker for working with Symfony.
* A great Symfony seed repo for anyone who wants to start their project.

### Quick start
**Make sure you have Docker version >= 17.04.0**

```bash
# clone our repo
# --depth 1 removes all but one .git commit history
git clone --depth 1 --recursive https://github.com/NicklasWallgren/symfony-docker-starter.git symfony-docker-starter

# change directory to our repo
cd symfony-docker-starter

# start the docker containers. The first boot will take some time
make
```
go to [http://localhost](http://localhost) or [http://<docker-machine>](http://<docker-machine>)

# Getting Started

## Commands

### Start containers
```bash
make

```
### Stop containers
```bash
make halt

```
### Start individual container
```bash
make start [php-fpm|php-cli|nginx|mysql|memcached]

```
### Stop individual container
```bash
make stop [php-fpm|php-cli|nginx|mysql|memcached]

```
### Update composer dependencies
```bash
make update-project

```
### Access Symfony cli
```bash
# Access the php container
make bash-cli
    
# Launch the symfony cli
php ./symfony/bin/console
```
### Access MySQL cli
```bash
make mysql-cli

```
### Access PHP container bash
```bash
make bash-php

```
### Access Nginx container bash
```bash
make bash-nginx

```
### Access PHP-FPM container bash
```bash
make bash-fpm

```
### Access Memcached container bash
```bash
make bash-memcached

```
### Access MySQL container bash
```bash
make bash-mysql

```
### Check container status
```bash
make status

```
# Contributing
I'll accept pretty much everything so feel free to open a Pull-Request





