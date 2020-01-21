# Micro-serviço com Node.js

- Utilizando Kafka e Node.js

## Aplicações

- API Principal (Station);
- Geração de certificado

## Fluxo

- API Principal envia uma mensagem pro serviço de certificado para gerar o certificado;
- Micro-serviço de certificado devolve uma resposta 

- Receber uma resposta assíncrona de quando o e-mail com certificado foi enviado;

## Requisitos

- Yarn
- Docker
- Docker Compose

## Rodando o projeto

Para subir o Kafka rode: `$ docker-compose up --build`

Para subir a api: 
`$ cd kafkanode/api`
`$ yarn dev`

Para subir o microserviço:
`$ cd kafkanode/certification`
`$ yarn dev`


## Executando

Faça uma requisição POST para: `http://localhost:3333/certifications`
