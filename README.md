# MySQL et PHPmyAdmin en container
![Static Badge](https://img.shields.io/badge/Version-1.0-blue) ![Docker Image Version (tag latest semver)](https://img.shields.io/docker/v/_/mysql/latest?logo=mysql&label=Mysql) ![Docker Image Version (tag latest semver)](https://img.shields.io/docker/v/_/phpmyadmin/latest?logo=phpmyadmin&label=PhpMyAdmin)



## Modifier le fichier .env.local avec le password de l'utilisateur root
```ini
#Fichier .env.local

MYSQL_HOST=%
MYSQL_ROOT_PASSWORD=mypassword
```

## Démarrer le container
```bash
#Démarrage du container

cd mysql-phpmyadmin-conainer
docker-compose up -d
```

## Ouvrir PhpMyAdmin
Dans le navigateur, aller sur http://localhost:9090

login `root` mdp `mypassword`

## Pour utiliser dans un projet de dev local

Fichier .env.local dans le projet qui utilise cette BDD :

```ini
DB_HOST=host.docker.internal # ou Localhost
DB_PORT=3640
DB_NAME=db_name # à modifier
DB_USER=root
DB_PASSWORD=mypassword # à modifier
```

![MacOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) ![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white
)
![Mysql](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white
)