# Django docker dev

[Docker compose](https://docs.docker.com/compose/) para desenvolvimento local de aplicações [Django](https://djangoproject.com)
usando [Postgresql](https://www.postgresql.org/), [Redis](https://redis.io/) e [RabbitMQ](https://www.rabbitmq.com/).

## Variáveis de ambiente

As variáveis de ambiente necessárias para execução dos serviços devem ser definidas em um arquivo `.env` na raiz
do projeto:

```bash
POSTGRES_DB=database
POSTGRES_USER=postgres
POSTGRES_PASSWORD=admin
POSTGRES_HOST=localhost
POSTGRES_PORT=5432

REDIS_PASSWORD=admin
REDIS_HOST=localhost
REDIS_PORT=6379

RABBITMQ_USER=rabbitmq
RABBITMQ_PASSWORD=admin
RABBITMQ_HOST=localhost
RABBITMQ_PORT=5672
```

## Execução dos serviços

Iniciar e subir os serviços:

```bash
docker compose up -d
```

Desligar os servicos:

```bash
docker compose down
```
