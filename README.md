<br />
<div align="center">
  <a href="https://github.com/timwassenburg/laravel-artisan-extender">
    <img src="img/wrench.png" alt="Logo" width=120>
  </a>

<h1 align="center">Laravel Artisan Extender</h1>

  <p align="center">
    A collection of generator packages to quickly generate services, actions, repositories, pivot tables, and traits for your projects!
  </p>
<br><br>
</div>

[![Latest Version on Packagist](https://img.shields.io/packagist/v/timwassenburg/laravel-artisan-extender.svg?style=flat-square)](https://packagist.org/packages/timwassenburg/laravel-artisan-extender)
[![Total Downloads](https://img.shields.io/packagist/dt/timwassenburg/laravel-artisan-extender.svg?style=flat-square)](https://packagist.org/packages/timwassenburg/laravel-artisan-extender)
[![License](https://img.shields.io/packagist/l/timwassenburg/laravel-artisan-extender)](https://packagist.org/packages/timwassenburg/laravel-artisan-extender)

## Table of Contents
  <ol>
    <li><a href="#installation">Installation</a></li>
    <li>
      <a href="#usage">Usage</a>
      <ul>
        <li><a href="#generate-services">Generate services</a></li>
        <li><a href="#generate-actions">Generate actions</a></li>
        <li><a href="#generate-repositories">Generate repositories</a></li>
        <li><a href="#generate-traits">Generate traits</a></li>
        <li><a href="#generate-pivot-tables">Generate pivot tables</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
  </ol>

## Installation
Install the package with composer.
```bash
composer require timwassenburg/laravel-artisan-extender
```

## Usage

### Generate services
To generate a new service use the following artisan command.

```bash
php artisan make:service UserService
```

Optionally, you can add multiple method names (seperated by comma) with the ```--methods``` param.

```bash
php artisan make:service UserService --methods=register,login,logout
```

[Click here to learn more about the Service Generator](https://github.com/timwassenburg/laravel-service-generator)

### Generate actions
Run the following command on the command-line to generate a new action.
```bash
php artisan make:action {name}
```
[Click here to learn more about the Action Generator](https://github.com/timwassenburg/laravel-action-generator)

### Generate repositories
Run the following command.
```bash
php artisan make:repository UserRepository
```
This example will generate the following files:
```bash
app\Repositories\Eloquent\UserRepository
app\Repositories\UserRepositoryInterface
```
[Click here to learn more about the Repository Generator](https://github.com/timwassenburg/laravel-repository-generator)

### Generate traits
Run the following command on the command-line to generate a new trait.
```bash
php artisan make:trait {name}
```
Optionally, you can add multiple method names (seperated by comma) with the ```--methods``` param.

[Click here to learn more about the Trait Generator](https://github.com/timwassenburg/laravel-trait-generator)

```bash
php artisan make:trait Notifiable --methods=notify,notifications
```

### Generate pivot tables
Run the following command on the command-line to generate a new migration for the pivot table.
```bash
php artisan make:pivot {first_table_name} {second_table_name}
```

The command will create a new migration in ```database/migrations```. Run the migrations to create the table.
```bash
php artisan migrate
```
[Click here to learn more about the Pivot Table Generator](https://github.com/timwassenburg/laravel-pivot-table-generator)

## Contributing
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
