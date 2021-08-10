# Tagando repositórios estrelados do GitHub
## Este projeto tem por objetivo criar um breve sistema backend que consome apis publicas do Github para adicionar tags a um repositório estrelado por um usuario Git

## Status do Projeto
<h4 align="center"> 
	Concluído 🚀
</h4>

### Features

- [x] Busca repositório estrelados de um usuário
- [x] Gerencia tags de repositórios(CRUD)
- [x] Filtrar repositórios por tags
- [x] Serviço que sugere tags mais utilizadas

### Pré-requisitos

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
[PHP](https://www.php.net/downloads) a versão utilizada para o desenvolvimento da aplicação foi a "PHP 7.3.29"
Em sistemas operacionais Linux ou Mac, a instalação do PHP é bastante simplificada, bastando apenas utilizar o comando de instalação:
Linux - sudo apt-get install php7.3
Mac - brew install php@7.3
No Windows, você precisará baixar e extrair o arquivo php-7.3.29-nts-Win32-VC15-x64.zip baixado no site do php.net. Em seguida, você deverá abrir o menu Iniciar e procurar por "Editar as variáveis de ambiente para a sua conta".

[sqlite] deve-se configurar a database utilizada na pasta do PHP, no nosso caso o SQLite
localizar a linha ";extension=pdo_sqlite" no arquivo php.ini e remover o ';'

[curl] habilitar o recurso de requisições.
adicionar a linha "extension=php_curl.dll" no arquivo php.ini

[composer](https://getcomposer.org/) a versão utilizada para o desenvolvimento da aplicação foi a "Composer version 2.1.5"
No Linux e no Mac, bastará copiar o código em "Command-line installation" e executá-lo no terminal. No Windows, basta baixar e executar o instalador Composer-Setup.exe.

### 🎲 Rodando o Back End (servidor)

```bash
# Clone este repositório
$ git clone <https://github.com/CasaDoSaber/challenge-alan-backend.git>

# Acesse a pasta do projeto no terminal/cmd
$ cd challenge-alan-backend\githubTagStar

# Instale as dependências
$ composerinstall

# Execute a aplicação em modo de desenvolvimento
$ php artisan serve

# O servidor inciará na porta:8000 - acesse <http://localhost:8000>
```

### 🛠 Tecnologias

As seguintes ferramentas foram usadas na construção do projeto:

- [PHP](https://www.php.net/)
- [Laravel](https://laravel.com/docs/5.8)
- [Sqlite](https://www.sqlite.org/index.html)
- [Api Rest](https://curl.se/)


