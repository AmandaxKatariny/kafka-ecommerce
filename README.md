# Curso Kafka - Alura

## Aula 01

O que aprendemos nessa aula:

- O que são produtores
- O que são consumidores
- Criação de tópicos manualmente
- Como instalar e rodar o Kafka

### Comandos utilizados 

- `bin/zookeeper-server-start.sh config/zookeeper.properties`
- `bin/kafka-server-start.sh config/server.properties` 
- `bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic LOJA_PEDIDO`
- `bin/kafka-topics.sh --list  --bootstrap-server localhost:9092`
- `bin/kafka-topics.sh --bootstrap-server localhost:9092 --describe`
- `bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic ECOMMERCE_NEW_ORDER --from-beginning`
- 