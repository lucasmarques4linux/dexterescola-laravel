# Instalar o Composer
https://github.com/Diego-Brocanelli/ambiente-dev-php-ubuntu

https://github.com/rhchristian/laravel-docs-pt-br

## For Linux using PHP 7:
sudo apt-get install php7.0-mbstring
sudo apt install php7.0-dom

## and don't forget to run:
sudo service apache2 restart

# Instalar o projeto do Laravel
composer create-project --prefer-dist laravel/laravel blog

composer create-project --prefer-dist laravel/laravel blog "5.4.*"

composer create-project laravel/laravel meu_projeto 5.2.x-dev

## Para instalar as dependencias
composer install

chmod para corrigir as permissões de usuário das pastas

php artisan key:generate

# Artisan
http://www.vedovelli.com.br/web-development/o-que-e-o-artisan/

http://laravel-docs-pt-br.readthedocs.io/en/5.0/artisan/

# Routes
php artisan route:list

# Blade
https://laravel.com/docs/5.5/blade

# Migrations
Setar o banco de dados no arquivo .ENV

```
DB_CONNECTION=pgsql
DB_HOST=127.0.0.1
DB_PORT=5432
DB_DATABASE=dexterescola
DB_USERNAME=linux
DB_PASSWORD=123
```

https://laravel.com/docs/5.5/migrations

php artisan make:migration create_alunos_table --create=alunos

php artisan migrate >> Roda as migrações

php artisan migrate:rollback >> Volta uma migrate.. Indice é o batch no banco de dados.

# Model
php artisan make:model Model/Aluno // Nome da tabela no singular - convenção

## Eloquent -> Active Record do Laravel

# Tinker
Interface de linha de comando para rodar a aplicação no terminal

$aluno = new App\Model\Aluno;      // Criando um aluno;
$aluno->atributo = "valor"                 // Adionando valores aos atributos.
$aluno->save()                                   // Salva no banco de dados

## License

The Laravel framework is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT).