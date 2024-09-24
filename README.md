# Shopware Setup with Docker and DDEV

## Requirements

* [Homebrew](https://brew.sh/) on Mac
* [Docker](https://www.docker.com/products/docker-desktop/)
* [DDEV](https://ddev.readthedocs.io/en/stable/)

<details>
    <summary>Installation on Mac</summary>

Install ddev with homebrew

```shell
brew install drud/ddev/ddev
```

#### Install mkcert

```shell
mkcert -install
```

</details>

## Setup

```shell
git clone https://github.com/pt1602/shopware-docker-ddev.git
cd shopware-docker-ddev
ddev start && ddev setup
```

* open https://shopware.ddev.site/
* Install Shopware 6 via default installer
* Activate the theme and needed plugins
* That should be it, happy coding

### Access

* https://shopware.ddev.site/

### Admin:

* https://shopware.ddev.site/admin

## Nice to know DDEV-Commands

<details>
    <summary>All you need to know</summary>

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
</details>
