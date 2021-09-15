# RabbitMQ with management and compatible version of the delayed message exchange plugin

### Running from docker hub
```
docker run heidiks/rabbitmq-delayed-message-exchange:latest
```

### Docker compose sample:

```
version: '3.3'

services:
  rabbit:
    image: heidiks/rabbitmq-delayed-message-exchange:latest
    environment:
      - RABBITMQ_DEFAULT_USER=admin
      - RABBITMQ_DEFAULT_PASS=password
    ports:
      - "5672:5672"
      - "15672:15672"
```

### Environment
The environment variables are the same as the [official image](https://hub.docker.com/_/rabbitmq/)
- Sample
    - RABBITMQ_DEFAULT_USER=admin
    - RABBITMQ_DEFAULT_PASS=password

[ref-url](https://github.com/heidiks/rabbitmq-delayed-message-exchange/blob/master/README.md)