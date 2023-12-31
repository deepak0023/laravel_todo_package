# Todo

### This package was mainly created for tesing how the larvel package scafolding and psr4 namespace works

### Steps to be followed

#### Install package

```bash
composer require deepak0023/todo
```

#### Create dummy database

- Get into mysql terminal
- Login with credentials

```bash
create database <database-name>
```

#### Add Service provider

- Inside config/app.php, add the follwing entries inside the provider array list

```bash
Deepak0023\Todo\TestServiceProvider::class
```

#### Update composer.json 

- Inside composer.json add the follwing entry inside autoload psr4 mapping

```bash
"Deepak0023\\Todo\\": "vendor/deepak0023/todo/src"
```

#### Publish package

- After hitting the command publish the pacakge for the above service provider

```bash
php artisan vendor publish
```

#### Migrate tables

```bash
php artisan migrate
```

#### Please add the following values in the .env with your name

```bash
TODO_NAME=<your-name>
```

### Features 

- Adding todo text to a dummy todos table

#### Enjoy !!!
