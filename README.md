## Tecnologias
 
- [Spring Boot](https://spring.io/projects/spring-boot)
- [Spring MVC](https://docs.spring.io/spring-framework/reference/web/webmvc.html)
- [Spring for Kafka](https://docs.spring.io/spring-kafka/reference/html/)
- [Kafka](https://kafka.apache.org)
- [Docker Compose](https://docs.docker.com/compose/)

## Como Executar

- Rodar o Kafka com o Docker Compose:
```
$ docker-compose up
```

- Adicionar /etc/hosts o hostname `kafka`.
- Clonar repositório git
- Construir o projeto:
```
$ ./mvnw clean package
```
- Executar a aplicação:
```
$ java -jar target/messaging-springboot-0.0.1-SNAPSHOT.jar
```

- Enviar um hello
```
$ curl http://localhost:8080/kafka/hello/lucas
```

- Visualizar mensagem recebida no log:
```
Consumer Message: Olá, lucas
```