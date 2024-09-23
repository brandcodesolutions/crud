1. Introdução:
Este projeto é um CRUD básico (Create, Read, Update, Delete) implementado com PHP, MySQL, HTML e CSS. Ele permite gerenciar uma lista de usuários com operações de banco de dados.

2. Requisitos:
PHP (7.0 ou superior)
MySQL
Servidor XAMPP ou WAMP
Editor VS Code
3. Configuração:
Banco de Dados:

Acesse phpMyAdmin via http://localhost/phpmyadmin.
Crie o banco de dados crud_db:
sql
Copiar código
CREATE DATABASE crud_db;
Crie a tabela users:
sql
Copiar código
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
4. Estrutura do Projeto:
bash
Copiar código
crud/
├── index.php        # Listagem de usuários
├── create.php       # Formulário de criação
├── update.php       # Edição de usuários
├── delete.php       # Exclusão de usuários
├── db.php           # Conexão com o banco
└── style.css        # Estilos
5. Descrição dos Arquivos:
db.php: Conexão com o banco de dados MySQL.
index.php: Página principal, lista usuários e oferece opções de edição e exclusão.
create.php: Formulário para adicionar novos usuários.
update.php: Formulário para editar um usuário existente.
delete.php: Lógica de exclusão de um usuário.
style.css: Estilos básicos de layout.
6. Uso:
Configure o projeto em um servidor local (XAMPP/WAMP).
Acesse index.php no navegador para visualizar a lista de usuários.
Use as opções para adicionar, editar e excluir registros.
Conclusão:
Este CRUD é uma aplicação simples para gerenciamento de dados, adequada para fins educacionais e implementação básica de operações com banco de dados.
