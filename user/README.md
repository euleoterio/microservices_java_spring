# Projeto User - Produtor de Mensagem

Este é um projeto Java que funciona como um produtor de mensagens. Ele foi desenvolvido utilizando Java 17, Maven, PostgreSQL, Spring Boot, Spring Web, Spring Data JPA, Spring Validation, Spring AMQP, RabbitMQ e CloudAMQP.

## Descrição

O projeto "user" é um produtor de mensagens que fornece APIs para interagir com um banco de dados PostgreSQL e enviar mensagens para uma fila RabbitMQ hospedada no serviço CloudAMQP.

## Pré-requisitos

Certifique-se de ter os seguintes pré-requisitos instalados em seu ambiente de desenvolvimento:

- Java 17
- Maven
- PostgreSQL
- RabbitMQ
- CloudAMQP (ou outro serviço de mensageria compatível com RabbitMQ)

## Configuração

Antes de iniciar o projeto, você precisará configurar as seguintes informações:

- Configurações do banco de dados PostgreSQL no arquivo `application.properties`.
- Configurações de conexão RabbitMQ no arquivo `application.properties`.

## Como Executar

Para executar o projeto, siga estas etapas:

1. Clone o repositório para o seu ambiente de desenvolvimento.
2. Configure as informações do banco de dados PostgreSQL e RabbitMQ no arquivo `application.properties`.
3. Certifique-se de ter um servidor PostgreSQL e um servidor RabbitMQ em execução.
4. Execute o seguinte comando na raiz do projeto:

```bash
mvn spring-boot:run
