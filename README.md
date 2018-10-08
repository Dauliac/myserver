# MyServer
My own docker-compose: Traeefik/nextcloud/wordpress infrastructure

## Getting started
### Install
- Install `docker`
- Install `docker-compose`
- Install `apache-utils`
- git clone

### Config
Copy file from exemple and fill them:
- Add SQL user and passwords in `src/mysql/default.sql`
- Add SQL user and passwords in `.env`
- Fill .env
- Update traefik api password with:
    ```
      htpasswd -bc ./src/traefik/htpasswd USER PASSWORD
    ```

### Start
Start docker-compose.yml:
```
    docker-compose up
```

Start wordpress-compose.yml:
```
    docker-compose up -f wordpress-compose.yml
```
