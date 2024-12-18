# Estacionamento Backend

**Descrição breve**: Este projeto é o backend para um sistema de gerenciamento de estacionamento, fornecendo APIs para operações como entrada e saída de veículos, cálculo de tarifas e disponibilidade de vagas.

## Índice

1. [Visão Geral](#visão-geral)
2. [Funcionalidades](#funcionalidades)
3. [Tecnologias Utilizadas](#tecnologias-utilizadas)
4. [Pré-requisitos](#pré-requisitos)
5. [Instalação](#instalação)
6. [Uso](#uso)
7. [Contribuindo](#contribuindo)
8. [Licença](#licença)

## Visão Geral

O Estacionamento Backend é responsável por gerenciar as operações de um estacionamento, incluindo:

- Registro de entrada e saída de veículos
- Cálculo automático de tarifas com base no tempo de permanência
- Monitoramento da disponibilidade de vagas
- Geração de relatórios operacionais

## Funcionalidades

- [x] Registro de entrada de veículos
- [x] Registro de saída de veículos
- [x] Cálculo de tarifas
- [x] Monitoramento de vagas disponíveis
- [x] Geração de relatórios (em desenvolvimento)

## Tecnologias Utilizadas

- **Linguagem**: TypeScript
- **Framework**: Node.js com Express
- **Banco de Dados**: PostgreSQL
- **ORM**: Prisma

## Pré-requisitos

Antes de começar, certifique-se de ter instalado em sua máquina:

- [Node.js](https://nodejs.org/) (versão 14 ou superior)
- [Docker](https://www.docker.com/) (para executar o banco de dados PostgreSQL)

## Instalação

1. Clone o repositório:

   ```bash
   git clone https://github.com/enricomadeu/estacionamento-backend.git
   ```

2. Acesse o diretório do projeto:

   ```bash
   cd estacionamento-backend
   ```

3. Instale as dependências:

   ```bash
   npm install
   ```

4. Configure o banco de dados:

   - Inicie o Docker e execute o comando para subir o container do PostgreSQL:

     ```bash
     docker-compose up -d
     ```

   - Execute as migrações do Prisma para configurar o banco de dados:

     ```bash
     npx prisma migrate dev
     ```

## Uso

1. Inicie o servidor de desenvolvimento:

   ```bash
   npm run dev
   ```

2. O backend estará disponível em `http://localhost:3000`.

3. Utilize ferramentas como [Postman](https://www.postman.com/) ou [Insomnia](https://insomnia.rest/) para testar as APIs disponíveis.

## Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e enviar pull requests. Para maiores detalhes, veja [CONTRIBUTING.md](CONTRIBUTING.md).

## Licença

Este projeto está sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.
