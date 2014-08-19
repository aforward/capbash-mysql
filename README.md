capbash-mysql
==============

Scripts for installing mysql, should be used in conjunction with capbash

# How to Install #

Install capbash first, more details at:
https://github.com/aforward/capbash

```
curl -s https://raw.githubusercontent.com/aforward/capbash/master/capbash-installer | bash
capbash new YOUR_REPO_ROOT
cd YOUR_REPO_ROOT
```

Now you can install mysql into your project

```
capbash install mysql
```

# Configurations #

The available configurations include:

```
MYSQL_DATA_DIR=${MYSQL_DATA_DIR-/var/apps/mysql/data}
MYSQL_PORT=${MYSQL_PORT-3306}
MYSQL_ADMIN_USERNAME=${MYSQL_ADMIN_USERNAME-admin}
MYSQL_ADMIN_PASSWORD=${MYSQL_ADMIN_PASSWORD-WNRfMarrXa74bT}
```

# Deploy to Remote Server #

To push the mysql script to your server, all you need if the IP or hostname of your server (e.g. 192.167.0.48) and your root password.

```
capbash deploy <IP> mysql
```

For example,

```
capbash deploy 127.0.0.1 mysql
```
