# Nome do Projeto: Biblioteca API (Gestão de Acervo)

## Integrantes do Grupo
1. [Augusto Rocha Silva - RM556316]
2. [Guilherme Vieira Augusto - RM557264]
3. [Erik Yuuta Goto - RM558076]
4. [Wendell dos Santos Silva - RM558859]

## Contexto do Projeto
- **O que é:** Uma API RESTful desenvolvida em C# .NET 10 para a gestão e controlo do catálogo de uma biblioteca.
- **Qual problema resolve:** Resolve a desorganização no controlo de acervos, substituindo processos manuais por um sistema automatizado que permite criar, consultar, atualizar e apagar registos de livros de forma estruturada.
- **Para quem é destinado:** Bibliotecários, administradores de instituições de ensino e aplicações de autoatendimento para alunos e leitores.

## Banco de Dados Utilizado
- **SQLite**
- A base de dados é gerada localmente num ficheiro (`biblioteca.db`) utilizando o Entity Framework Core como ORM, o que permite executar o projeto em qualquer computador sem a necessidade de instalar um servidor de base de dados externo.

## Endpoints Disponíveis

| Rota (Endpoint) | Método HTTP | Descrição |
|---|---|---|
| `/api/v1/livros` | **GET** | Retorna a lista de todos os livros registados no acervo (Status 200). |
| `/api/v1/livros/{id}` | **GET** | Retorna os detalhes de um livro específico utilizando o seu ID (Status 200 ou 404). |
| `/api/v1/livros` | **POST** | Regista um novo livro na base de dados (Status 201 ou 400). |
| `/api/v1/livros/{id}` | **PUT** | Atualiza as informações de um livro já existente (Status 204, 400 ou 404). |
| `/api/v1/livros/{id}` | **DELETE** | Remove permanentemente um livro do sistema (Status 204 ou 404). |


## Instruções para Rodar o Projeto Localmente
**Pré-requisitos:** SDK do .NET (versão 10 ou compatível) instalado.

1. Clona este repositório para a tua máquina:
   ```bash
   git clone [URL-DO-TEU-REPOSITORIO]