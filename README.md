# Django + MySQL in Docker 

This is new project template


## Passwords

Passwords in .env:

```
MYSQL_DATABASE=db_django
MYSQL_USER=web_django
MYSQL_PASSWORD=password
MYSQL_ROOT_PASSWORD=password
```

## Restore MySQL premissions

db_access,sql

```
grant all on db_django.* to 'web_django'@'%';
flush privileges;
```


## Scripts
```
0-init.sh         - build container
1-run.sh          - run container
2-up.sh           - run container (up)
3-rebuild.sh      - rebuild container
4-migrate-db.sh   - migrate Django DB
5-mysql-shell.sh  - MySqql interactive root shell
6-django-shell.sh - Django shell
7-down.sh         - shutdown container
```
