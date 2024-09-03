Enunciado
Objetivo: Criar e gerenciar um banco de dados para uma biblioteca.

Passos:

Criar o Banco de Dados: Nomeie o banco de dados como Biblioteca.
Criar Tabelas:
Autores: Armazena informações sobre autores.
AutorID (INT, AUTO_INCREMENT, PRIMARY KEY)
Nome (VARCHAR(100), NOT NULL)
Nacionalidade (VARCHAR(100))
Livros: Armazena informações sobre livros.
LivroID (INT, AUTO_INCREMENT, PRIMARY KEY)
Titulo (VARCHAR(255), NOT NULL)
AutorID (INT, FOREIGN KEY referenciando Autores(AutorID))
AnoPublicacao (YEAR)
Genero (VARCHAR(50))
Emprestimos: Armazena informações sobre os empréstimos de livros.
EmprestimoID (INT, AUTO_INCREMENT, PRIMARY KEY)
LivroID (INT, FOREIGN KEY referenciando Livros(LivroID))
DataEmprestimo (DATE, NOT NULL)
DataDevolucao (DATE)
NomeUsuario (VARCHAR(100), NOT NULL)
Inserir Dados:
Adicionar autores à tabela Autores.
Adicionar livros à tabela Livros.
Adicionar registros de empréstimos à tabela Emprestimos.
Excluir Dados:
Remover um livro e o empréstimo relacionado a ele.

# Banco de Dados Biblioteca

Este projeto cria e gerencia um banco de dados para uma biblioteca, permitindo a administração de autores, livros e empréstimos.

## Estrutura do Banco de Dados

### Tabelas

1. **Autores**
   - `AutorID` (INT, AUTO_INCREMENT, PRIMARY KEY)
   - `Nome` (VARCHAR(100), NOT NULL)
   - `Nacionalidade` (VARCHAR(100))

2. **Livros**
   - `LivroID` (INT, AUTO_INCREMENT, PRIMARY KEY)
   - `Titulo` (VARCHAR(255), NOT NULL)
   - `AutorID` (INT, FOREIGN KEY referenciando `Autores(AutorID)`)
   - `AnoPublicacao` (YEAR)
   - `Genero` (VARCHAR(50))

3. **Emprestimos**
   - `EmprestimoID` (INT, AUTO_INCREMENT, PRIMARY KEY)
   - `LivroID` (INT, FOREIGN KEY referenciando `Livros(LivroID)`)
   - `DataEmprestimo` (DATE, NOT NULL)
   - `DataDevolucao` (DATE)
   - `NomeUsuario` (VARCHAR(100), NOT NULL)

## Operações

1. **Criação do Banco de Dados e Tabelas**

   Execute o script SQL para criar o banco de dados `Biblioteca`, as tabelas `Autores`, `Livros`, e `Emprestimos`.

2. **Inserção de Dados**

   Execute os comandos SQL fornecidos para inserir dados de exemplo nas tabelas.

3. **Exclusão de Dados**

   Para excluir um livro e o empréstimo relacionado, use os comandos SQL fornecidos.

## Executando o Script SQL

1. Conecte-se ao servidor MySQL.
2. Copie e cole o código SQL fornecido em um cliente MySQL.
3. Execute o script para criar e gerenciar o banco de dados `Biblioteca`.

## Notas

- Certifique-se de que o banco de dados e as tabelas estejam limpos antes de executar os comandos de inserção e exclusão para evitar conflitos.

