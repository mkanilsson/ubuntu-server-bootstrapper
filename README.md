# Ubuntu Server Bootstrapper

Ubuntu Server Bootstrapper is a small shell script made for a faster
installation and setup of an Ubuntu server.

This script is designed for Laravel projects,
but can be used for webservers no-matter language!

## Install

> Always check script's from the internet before running
> them, especially if they require root!

On Ubuntu as root, Run:

```bash
wget https://raw.githubusercontent.com/Jrp0h/ubuntu-server-bootstrapper/master/ubuntu-server-bootstrapper.sh

chmod +x ubuntu-server-bootstrapper.sh

./ubuntu-server-bootstrapper.sh
```

Then just follow the instructions!

## What does Ubuntu Server Bootstrapper do?

It installs programs(list of programs can be found below) and
configures nginx, ssh and a firewall(ufw).

## Software the script installs

### Programs

All the programs and why they are needed.
Of course more programs and libraries have been install,
but these are the once that are explicitly downloaded and installed.

* dialog - UI for the script
* nginx - Webserver
* Postgresql - Database
* Redis - Cache
* ufw - Firewall
* fail2ban - Security
* Composer - Good for Laravel
* npm - Good for Laravel
* node - Good for Laravel
* Certbot (Let's Encrypt) - SSL certificate for webserver
* PHP - Dependency of composer and laravel
* zip - Dependency of composer
* unzip - Dependency of composer

### PHP Extensions

* php-fpm
* php-pgsql
* php-mbstring
* php-dom
* php-redis
* php-dev
* php-pear
* php-gd

## Future Goals

* Customize software
  * apache vs nginx
  * postgresql vs mysql vs mariadb vs mongodb
* Better support for other languages
  * NodeJS
    * pm2
  * Ruby
  * Go
  * Rust
  * Crystal
  * Python
* Better security
  * Create database users
