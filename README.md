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

```sh
php artisan migrate
```

Execute o semeador de banco de dados:

```sh
php artisan db:seed
```

> **Note**  
> If you get an "Invalid datetime format (1292)" error, this is probably related to the timezone setting of your database.  
> Please see https://dba.stackexchange.com/questions/234270/incorrect-datetime-value-mysql


Create a symlink to the storage:

```sh
php artisan storage:link
```

Run the dev server (the output will give the address):

```sh
php artisan serve
```

You're ready to go! Visit the url in your browser, and login with:

-   **Username:** admin@filamentphp.com
-   **Password:** password

## Features to explore

### Relations

#### BelongsTo
- ProductResource
- OrderResource
- PostResource

#### BelongsToMany
- CategoryResource\RelationManagers\ProductsRelationManager

#### HasMany
- OrderResource\RelationManagers\PaymentsRelationManager

#### HasManyThrough
- CustomerResource\RelationManagers\PaymentsRelationManager

#### MorphOne
- OrderResource -> Address

#### MorphMany
- ProductResource\RelationManagers\CommentsRelationManager
- PostResource\RelationManagers\CommentsRelationManager

#### MorphToMany
- BrandResource\RelationManagers\AddressRelationManager
- CustomerResource\RelationManagers\AddressRelationManager
