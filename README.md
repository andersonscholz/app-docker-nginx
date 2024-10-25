# Nginx Node.js API com RabbitMQ

Este projeto consiste em uma aplicação que utiliza Nginx como servidor web reverso, Node.js para a API e RabbitMQ para gerenciamento de filas de mensagens.

## Índice

- [Sobre](#sobre)
- [Tecnologias](#tecnologias)
- [Pré-requisitos](#pré-requisitos)
- [Como Executar](#como-executar)
- [Acessando a API](#acessando-a-api)
- [Acessando o RabbitMQ](#acessando-o-rabbitmq)
- [Licença](#licença)

## Sobre

Este projeto utiliza Docker para subir as aplicações, onde a API possui um endpoint `/api/reset-password` que envia uma mensagem para uma fila no RabbitMQ, simulando uma solicitação de redefinição de senha. 

## Tecnologias

Este projeto utiliza as seguintes tecnologias:

- **Node.js**: Para a API.
- **Express**: Framework para a construção da API.
- **RabbitMQ**: Sistema de gerenciamento de filas de mensagens.
- **Docker**: Para containerização da aplicação.
- **Nginx**: Como servidor web reverso.

## Pré-requisitos

Antes de começar, você precisa ter instalado em sua máquina:

- [Docker](https://docs.docker.com/get-docker/) (versão 20 ou superior)
- [Docker Compose](https://docs.docker.com/compose/install/) (versão 1.27 ou superior)

## Como Executar

Siga os passos de [passos.txt](/passos.txt) para a criação e execução do projeto em sua máquina.

## Acessando a API

Após a inicialização, você pode acessar a API no seguinte endereço:

- **API**: [http://localhost/api/reset-password](http://localhost/api/reset-password)

## Acessando o RabbitMQ

Acesse a interface de gerenciamento do RabbitMQ em:

- **RabbitMQ**: [http://localhost:15672](http://localhost:15672)

Credenciais padrão:

- **Usuário**: `anderson`
- **Senha**: `anderson`

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).
