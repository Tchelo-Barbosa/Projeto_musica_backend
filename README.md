# Sistema Musical 

> Aplicação web em PHP Native e MySQL para gerenciamento completo de acervo musical, artistas, capas e integração com o YouTube.

---

## Sobre & Funcionalidades

Sistema responsivo para cadastro e controle de catálogo musical com foco em segurança e boa organização de dados.

*  Autenticação & Segurança:** Login/Logout com sessões (`$_SESSION`), senhas criptografadas com **BCrypt**, proteção contra **SQL Injection** (*Prepared Statements*) e **XSS** (`htmlspecialchars`).
*  Gestão de Artistas (CRUD):** Cadastro, listagem, edição, exclusão e upload de fotos com redimensionamento automático via PHP GD.
*  Gestão de Músicas (CRUD):** Vínculo por chave estrangeira (`artista_id`), upload de capas e extração automática de ID de vídeos do YouTube (`watch`, `embed`, `youtu.be`).
*  Biblioteca Musical:** Listagem geral com filtros dinâmicos por **busca textual**, **artista** e **gênero**.

---
# Tecnologias

* **Backend:** PHP 8.x
* **Banco de Dados:** MySQL / MariaDB
* **Mídia:** Extensão PHP GD
* **Frontend:** HTML5 & CSS3 puro

---

## Estrutura do Projeto

```text
sistema-musical/
├── bd.sql                    Script de criação do banco e tabelas
├── conexao.php               Conexão MySQLi e criação de diretórios
├── valida_sessao.php         Proteção de rotas autenticadas
├── login.php / logout.php    Autenticação de usuários
├── index.php                 Painel principal
├── cadastro_artista.php      CRUD de Artistas + Upload
├── cadastro_musica.php       CRUD de Músicas + YouTube
├── listagem_musicas.php      Biblioteca com filtros dinâmicos
└── styles.css                Estilização global
```


<p align="center">
  <img src="https://raw.githubusercontent.com/Tchelo-Barbosa/Projeto_musica_backend/main/assets_readme/laptop.gif" width="200" alt="Gato programador">
</p>
