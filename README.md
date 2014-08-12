capbash-mysql
==============

Scripts for installing mysql, should be used in conjunction with capbash

# How to Install #

Install capbash first, more details at:
https://github.com/aforward/capbash

```
git clone https://github.com/aforward/capbash YOUR_REPO_ROOT
cd YOUR_REPO_ROOT
./bootstrap
```

Now you can install mysql into your project

```
./capbash install mysql
```

# Configurations #

The available configurations include:

```
MYSQL_VERSION=${MYSQL_VERSION-5.0.96}
```

# Deploy to Remote Server #

To push the mysql script to your server, all you need if the IP or hostname of your server (e.g. 192.167.0.48) and your root password.

```
./capbash deploy <IP> mysql
```

For example,

```
./capbash deploy 127.0.0.1 mysql
```
