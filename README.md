# Shopware Setup with Docker and DDEV

## Requirements

* Homebrew on Mac
* Local Docker and DDEV installation

* Get Docker [here](https://www.docker.com/products/docker-desktop/)
* Get Homebrew [here](https://brew.sh/)

### Install ddev with homebrew

```shell
brew install drud/ddev/ddev
```

#### Install mkcert

```shell
mkcert -install
```

## Setup

```shell
ddev start && ddev setup
```

* open https://shopware.ddev.site/
* Install Shopware 6 via default installer
* Make sure you land on the https version after the installation
* Activate the theme and needed plugins
* That should be it, happy coding

### Access
* https://shopware.ddev.site/

### Admin:
* https://shopware.ddev.site/admin

## Nice to know DDEV-Commands

### Start container in current directory

```shell
ddev start
```

### Shutdown container in current directory

```shell
ddev stop
```

### Shutdown all containers

```shell
ddev poweroff
```

### Delete current container

```shell
ddev delete -O
```

### SSH

```shell
ddev ssh
```

### PhpMyAdmin

```shell
ddev phpmyadmin
```

### Mailpit

```shell
ddev launch -m
```

### Import db

```shell
ddev import-db --src=dump.sql.gz
```

### Export db

```shell
ddev export-db > dump.sql.gz
```
