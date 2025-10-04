---
title: "mysql"
draft: false
---

# mysql

## Establish connection to database

```bash
mysql -S /<pfad zum Socket>/mysql.sock
```

## Create database

```bash
create database grafana CHARACTER SET 'utf8mb4';
```

## Create user for database

```bash
create user 'grafana'@'%' identified by '<KENNWORT>';
```

## Grant users access to the database

```bash
grant all privileges on grafana.* to 'grafana'@'%';
```

## Enable permissions

```bash
flush privileges;
```

## Disconnect from database

```bash
quit
```
