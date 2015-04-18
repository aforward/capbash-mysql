capbash-mysql
==============

Scripts for installing mysql, should be used in conjunction with capbash

# How to Install #

Install capbash first, more details at:
https://github.com/capbash/capbash

```
curl -s https://raw.githubusercontent.com/capbash/capbash/master/capbash-installer | bash
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
MYSQL_LAUNCHER_DIR=${MYSQL_LAUNCHER_DIR-/var/local/mysql}
MYSQL_DATA_DIR=${MYSQL_DATA_DIR-${MYSQL_LAUNCHER_DIR}/data}
MYSQL_PORT=${MYSQL_PORT-3306}
MYSQL_ADMIN_USERNAME=${MYSQL_ADMIN_USERNAME-admin}
MYSQL_ADMIN_PASSWORD=${MYSQL_ADMIN_PASSWORD-yth3fn0t}
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
