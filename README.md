/docker-projeto1-dio/docker-compose.yml

---
# Projeto Docker-Compose - [Meu Curriculo](https://github.com/assisberlanda)

## Nessa projeto subo um container chamado my-apache-app
    version: '3.9'
      services:
        apache:
          image: httpd:latest
          container_name: my-apache-app
          ports:
          - '80:80'
          volumes:
          - ./website:/usr/local/apache2/htdocs
### na pasta /website - Coloquei os arquivo:
  - index.html
  - styles.css
  - assets/img/<varias imagens>
  
