# ProjetoCRUD
Projeto CRUD

Para rodar somente é necessário fazer o download do node modules e o mysql esta configurado como usuario root e senha root

-- Criação do banco de dados
CREATE DATABASE IF NOT EXISTS crud;
USE crud;

-- Criação da tabela users
CREATE TABLE IF NOT EXISTS users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    email VARCHAR(100) NOT NULL UNIQUE,
    pswd VARCHAR(100) NOT NULL
);

-- Inserção de dados exemplo
INSERT INTO users (nome, email, pswd) VALUES
('henrique', '1@email.com', 'asd'),
('Alice Silva', 'alice@email.com', 'senha123'),
('Bruno Costa', 'bruno@email.com', 'abc123'),
('Carla Silva', 'carla@email.com', '123'),
('Diego Souza', 'diego@email.com', '123senha'),
('Eduarda Lima', 'eduarda@email.com', 'edu321'),
('Felipe Rocha', 'felipe@email.com', 'senha456'),
('Gabriela Nunes', 'gabriela@email.com', 'gabi789'),
('Henrique Martins', 'henrique@email.com', 'sdf'),
('Isabela Fernandes', 'isabela@email.com', 'isa987'),
('João Pedro', 'joao@email.com', 'joao654'),
('Alex Silva', 'alex@email.com', 'senha123');

Este é um sistema web de gerenciamento de usuários . O objetivo do projeto é permitir o cadastro, edição, exclusão e visualização de usuários de forma prática e intuitiva.

A aplicação foi construída utilizando tecnologias modernas para garantir uma boa experiência tanto no uso quanto no desenvolvimento. O frontend foi feito com React e estilizado com Tailwind CSS, oferecendo uma interface clara e responsiva. No backend, foi utilizado Node.js com Express, responsável pelo processamento das requisições e comunicação com o banco de dados. Toda a persistência dos dados é feita em um banco MySQL, estruturado para armazenar as informações dos usuários de forma organizada.
