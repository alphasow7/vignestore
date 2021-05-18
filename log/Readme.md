# Projet-résumé


1- lancer en front-ground:
    -   docker-compose up -d app
    -   docker-compose up -d mysql
    -   docker-compose up -d phpmyadmin
    -   docker-compose up -d elasticsearch


Access: log
2- lancer logstash_log:
    
    docker-compose up --force-recreate logstash_log


3- Business logs:
    -   lancer logstash_bus_log:    docker-compose up --force-recreate logstash_bus_log

    -   lancer l'application:       docker exec -ti log_app_1 sh

    générer les evenement(logs):    php bin/console app:submit-events  






