# Larave Inertia Vue - Boilerplate

#### This is a boiler plate for laravel , inertia , vue - monorepo

### Pre requisite

1. composer 
2. node
3. npm

### Stack

- Laravel 11
- Vue 3
- Inertia
- Tailwind

### Steps

#### Below are the steps to run the app

###### Install php laravel dependencies
```bash
composer install
```

###### Install node modules
```bash
npm install && npm run dev
```

###### create env
```bash
cp .env.example .env
```

###### setup app key
```bash
php artisan key:generate
```

###### run migration
```bash
php artisan migrate
```

###### serve app
```bash
php artisan serve
```

- Open http://localhost:8000 or your predefined localhost route for viewing the website
