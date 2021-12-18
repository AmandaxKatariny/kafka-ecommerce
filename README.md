# Curso Kafka - Alura

## Aula 01 - Produtores e Consumidores

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

## Aula 02 - Paralelizando Tarefas em um serviço

O que aprendemos nessa aula:

- Como rodar diversos consumidores no mesmo grupo
- Como paralelizar tarefas
- A importância da chave para hash
- Cuidado com poll longo

### Comandos utilizados

- `/bin/kafka-topics.sh --alter --bootstrap-server localhost:9092 --topic ECOMMERCE_NEW_ORDER --partitions 3`
- `bin/kafka-topics.sh --bootstrap-server localhost:9092 --describe`


## Aula 03 - Criando nossa camada

O que aprendemos nessa aula:

- A importância de evitar copy e paste
- Criando nossa camada de abstração
- Criando nosso Dispatcher
- Criando nosso Service

## Aula 04 - Serialização customizada

O que aprendemos nessa aula:

- Como limpar os diretórios de log e dados do zookeeper e kafka
- Como utilizar diretórios não temporátios para o zookeeper e kafka
- Como utilizar o GSON
- Criando um serializador customizado do Kafka
- Verificar o conteúdo exato de uma mensagem em um programa
- Deserialização customizada
- Lidando com customização por serviço

