# docker-phpmyadmin-mariadb-mailhog
Docker Phpmyadmin - Mariadb - Mailhog (for SMTP localhost)
  - change database name -> line 21 in docker-compose.yml 'mydatabase'
  - change username -> line 22 in docker-compose.yml 'root'
  - change password -> line 23 in docker-compose.yml 'root'

# Start Docker
  - docker-compose up -d
  
#Access PHPMYADMIN
  - Go on localhost:8080
  -       environment:
            - MYSQL_ROOT_PASSWORD=root
            - MYSQL_DATABASE=mydatabase
            - MYSQL_USER=root
            - MYSQL_PASSWORD=root
  
  - Serveur : empty
  - user : root
  - password : root
            
            
#Access MailHog
  - Go on localhost:8081