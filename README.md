# Aplicativo de demonstração de filament

Um aplicativo de demonstração para ilustrar como o Filament Admin funciona.

![Aplicativo de demonstração de filament](https://github.com/filamentphp/demo/assets/171715/899161a9-3c85-4dc9-9599-13928d3a4412)

## Instalação

Clone o repositório localmente:

```sh
git clone https://github.com/AiltonDaSilva10/laravel-filament-demo.git filament-demo
```

Entrar na pasta do projecto 'filament-demo':

```sh
cd filament-demo
```

Instalar dependências do PHP:

```sh
composer install
```

Configuração de instalação:

```sh
cp .env.example .env
```

Gerar chave da aplicação:

```sh
php artisan key:generate
```

> **NOTA**  
> Configure as informações do banco de dados e acordo com as informações de seu servidor de banco de dados

Executar migrações de banco de dados:

```sh
php artisan migrate
```

Execute o semeador de banco de dados:

```sh
php artisan db:seed
```

Crie um link simbólico para o armazenamento das imagens:

```sh
php artisan storage:link
```

Execute o servidor de desenvolvimento:

```sh
php artisan serve
```
Você está pronto para ir! Visite a url (http://127.0.0.1:8000/) no seu navegador e faça login com:

-   **Nome de usuário:** admin@filamentphp.com
-   **Senha:** password
