<h1 align="center">
    Url Shortener
</h1>

API que encurta uma Url dada e salva ela por 5 minutos no Mongodb.

## Tecnologias

- Spring Boot
- Mongodb

## Como executar

- Clonar repositório git
- Iniciar Mongodb:
~~~~
cd ./docker
docker compose up
~~~~
- Construir projeto:
~~~~
mvn clean package
~~~~
- Executar a aplicação:
~~~~
java -jar target/urlshortener-0.0.1-SNAPSHOT.jar
~~~~

A API poderá ser acessada em [localhost:8080](https://localhost:8080).

## API Endpoints

Para fazer as requisições foi utilizado a ferramenta [Postman](https://www.postman.com/)

- Criar Url:
~~~~
POST localhost:8080/shorten-url

body:
{
    "url": "https://google.com"
}

response:
{
    "url": "http://localhost:8080/FP9YwoMEc"
}
~~~~

Para testar, basta copiar a Url que veio na resposta da requisição e colar no navegador.