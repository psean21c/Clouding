

### Messaging with RabbitMQ (SpringBoot)
[Spring Site: RabbitMQ](https://spring.io/guides/gs/messaging-rabbitmq/)



    compile (org.springframework.amqp:spring-rabbit:1.7.0.RELEASE)
    compile (org.springframework.amqp:spring-amqp:1.7.0.RELEASE)
    

```yml
#application-dev.yml

app:
  documan:  
    rabbitmq:
      connection:
        username: user
        password: user
        hostname: localhost
      queues:
        documan: Documan
      exchanges: 
        intercom: intercom
      routingKeys:
        documanRequiredFiles: documan.required.files

```
