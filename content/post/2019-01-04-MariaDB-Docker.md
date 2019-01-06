---
author: bing0ne
date: "2019-01-05T22:47:30-05:00"
slug: "mariadb-docker"
title: "How to install and Using MariaDB via Docker in Mac OS X"
tags: ["Env"]
description: "How to install MariaDB via Docker in Mac OS X "
showtoc: true
categories: ["Dev"]
---

## Pull Image 
I directly pull official MariaDB image. 
```shell
$ docker pull mariadb
```

## Run Container and Mapping Port
We need publish our port in container to host port.

```shell
$ docker run -p 3306:3306 --name some-mariadb -e MYSQL_ROOT_PASSWORD=my-secret-pw -d mariadb:latest
```

* `-p 3306:3306` publish port in container to host.
* `-d` will start our container in detached mode. 
* `--name` set a name for our container.
* `-e MYSQL_ROOT_PASSWORD` set a password for *root*

## Access Mysql
Firstly, we can access container shell. 
```shell
$ docker exec -it some-mariadb bash
```

Secondly, access the MariaDB in container via `mysql-client`.
```shell
$ mysql -uroot -p
```

