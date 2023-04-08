# docker-compose-app-dio
Esse é meu primeiro desafio docker, solicitado pelo bootcamp da DIO.

Utilizando o compose:
Primeiramente, dentro do diretório "meu-projeto", criei o arquivo com nano compose.yml possuindo o seguinte código:
version: '3.9'
services: apache
  image: httpd:latest
  container_image: meu-app
  ports:
  - '80:80'
  volumes:
  - ./website:usr/local/apache2/htdocs


Depois, criei o diretório website usando o comando mkdir website, ao entrar neste diretório pude criar meu arquivo html simples com nano index.html, possuindo o código:
   <html>
  <head>
    <h1> Funciona?</h1>
    <h2> Sim! </h2>
    
    </html>
  
  Por ultimo, descobrindo o ip com "ip a", pude entrar em minha aplicação indicando a porta anteriormente citada (80).
  
