# Desenvolvimento de Aplicações com Apache Kafka e .NET Core

Este repositório contém o código fonte relacionado ao módulo "Desenvolvimento de Aplicações com Apache Kafka e .NET Core" do curso "Desenvolvimento de Aplicações Escaláveis com Apache Kafka e .NET Core".

## Descrição do Módulo

Aplicação que implementa o Apache Kafka em conjunto com o framework .NET Core. Como integrar o Kafka em suas aplicações .NET Core e como implementar produtores e consumidores de mensagens Kafka para comunicação assíncrona e distribuída.

## Como Iniciar o Kafka e Zookeeper com o Docker Compose

1. Rode os containers usando o arquivo docker compose:

   ```bash
   docker-compose up -d
2. Visualize os container rodando:

   ```bash
   docker ps
3. Entrar dentro do container kafka:

   ```bash
   sudo docker exec -it kafka /bin/bash
4. Listar tópicos:

   ```bash
   kafka-topics --list --bootstrap-server localhost:9092
5. Criar tópico:

   ```bash
   kafka-topics --create --bootstrap-server localhost:9002 --replication-factor 1 --partitions 1 --topic tp-order
5. Consumir tópico:

   ```bash
   kafka-console-consumer  --bootstrap-server localhost:9092 --topic tp-order --from-be
   ginning
## Como executar o produtor (fazer pedido) e consumidor (notificar pedido)

1. Vá na aba Run/Debug do VSCODE e execute os dois projetos (Consolse e Api):
