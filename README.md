# MySQL et PHPmyAdmin en container

## Modifier le fichier .env.local avec le password de l'utilisateur root
```json
// Créer un fichier .env.local
MYSQL_HOST=%
MYSQL_ROOT_PASSWORD=mypassword
```

```bash
cd mysql-phpmyadmin-conainer
docker-compose up -d
```

Dans le navigateur, aller sur `http://localhost:9090`

login `root` mdp `mypassword`

Fichier .env.local dans le projet qui utilise cette BDD :

```ini
DB_HOST=host.docker.internal
DB_PORT=3640
DB_NAME=db_name # à modifier
DB_USER=root
DB_PASSWORD=mypassword
```