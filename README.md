# Gerador de CRUDs

[![Build Status](https://travis-ci.org/appzcoder/crud-generator.svg)](https://travis-ci.org/appzcoder/crud-generator.svg)
[![Total Downloads](https://poser.pugx.org/appzcoder/crud-generator/d/total.svg)](https://packagist.org/packages/appzcoder/crud-generator)
[![Latest Stable Version](https://poser.pugx.org/appzcoder/crud-generator/v/stable.svg)](https://packagist.org/packages/appzcoder/crud-generator)
[![License](https://poser.pugx.org/appzcoder/crud-generator/license.svg)](https://packagist.org/packages/appzcoder/crud-generator)

## Isto é um fork do
https://github.com/sohelamin/crud-generator

Mas usando o release 3.3.1, que usa Bootstrap


This Generator package provides various generators like CRUD, API, Controller, Model, Migration, View for your painless development of your applications.

## Requirements
    Laravel >= 5.3
    PHP >= 5.6.4

## Installation
```bash
composer create-project --prefer-dist laravel/laravel crud
cd crud

composer require ribafs/crud-generator --dev

php artisan vendor:publish --provider="Ribafs\CrudGenerator\CrudGeneratorServiceProvider"

php artisan crud:generate Cadastros --fields='title#string; body#text;' --controller-namespace=App\\Http\\Controllers \
 --form-helper=html

Add ao routes/web.php
Route::resource('/cadastros', 'App\Http\Controllers\CadastrosController');

Executar
php artisan route:clear

php artisan migrate

php artisan serve

http://127.0.0.1:8000/cadastros
```

## Documentation
Go through to the [detailed documentation](doc#readme)

## Screencast

[![Screencast](http://img.youtube.com/vi/831-PFBsYfw/0.jpg)](https://www.youtube.com/watch?v=K2G3kMQtY5Y)

#### If you're still looking for easier one then try this [Admin Panel](https://github.com/appzcoder/laravel-admin)

## Author

[Sohel Amin](http://sohelamin.com) :email: [Email Me](mailto:sohelamincse@gmail.com)

## License

This project is licensed under the MIT License - see the [License File](LICENSE) for details
