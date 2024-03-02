### Pour initier un nouveau projet :
1. Vérifier que tous les conteneurs sont coupé (pour libérer les ports)
```
cp docker-compose.yml nom-du-projet/docker-compose.yml
cd nom-du-projet/
docker-compose up -d
```

### Arrêter de travailler sur un projet :
`docker-compose down`

### Lister les contenueurs actifs
`docker ps -a`

### Stopper un conteneur
`docker stop nom-du-conteneur`

### Supprimer un conteneur
`docker rm -v nom-du-conteneur`

### Entrer dans le conteneur
`docker-compose exec -u www-data php /bin/bash`

### Recontruire les conteneurs après avoir modifié la configuration
`docker build -t docker-php-emsquared .`

### Intéragir avec une base de données dans le conteneur mysql
`mysql -h 127.0.0.1 -u root -pfubar`
