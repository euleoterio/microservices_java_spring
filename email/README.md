# Projeto Email - Consumidor e Envio de E-mails

Este é um projeto Java que funciona como um consumidor de mensagens e envia e-mails. Ele foi desenvolvido utilizando Java 17, Maven, PostgreSQL, Spring Boot, Spring Web, Spring Data JPA, Spring Validation, Spring AMQP, Spring Mail, RabbitMQ, CloudAMQP e SMTP Gmail.

## Descrição

O projeto "email" é um consumidor de mensagens que consome mensagens de uma fila RabbitMQ hospedada no serviço CloudAMQP. Além disso, ele também fornece funcionalidades para enviar e-mails usando o SMTP do Gmail.

## Pré-requisitos

Certifique-se de ter os seguintes pré-requisitos instalados em seu ambiente de desenvolvimento:

- Java 17
- Maven
- PostgreSQL
- RabbitMQ
- CloudAMQP (ou outro serviço de mensageria compatível com RabbitMQ)
- Conta de e-mail do Gmail (para enviar e-mails via SMTP)

## Configuração

Antes de iniciar o projeto, você precisará configurar as seguintes informações:

- Configurações do banco de dados PostgreSQL no arquivo `application.properties`.
- Configurações de conexão RabbitMQ no arquivo `application.properties`.
- Configurações do Spring Mail (SMTP Gmail) no arquivo `application.properties`.
- Certifique-se de configurar o arquivo `application-dev.properties` com informações sensíveis (como senhas) e adicione-o ao `.gitignore` para evitar que ele seja versionado.

## Como Executar

Para executar o projeto, siga estas etapas:

1. Clone o repositório para o seu ambiente de desenvolvimento.
2. Configure as informações do banco de dados PostgreSQL, RabbitMQ e SMTP Gmail no arquivo `application.properties`.
3. Certifique-se de ter um servidor PostgreSQL, um servidor RabbitMQ e uma conta de e-mail do Gmail configurada.
4. Execute o seguinte comando na raiz do projeto:

```bash
mvn spring-boot:run
