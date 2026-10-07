# E-Library IT

A digital library web application for browsing books and managing borrowing. Visitors explore the catalog by category or author. Members borrow books. Admins manage the whole collection from a dashboard.

## Features

- **Book hall (catalog):** browse books with SEO-friendly slugs, filtered by **author** or **category**
- **Authentication:** registration and login for members
- **Borrowing system:** borrow books and view your borrowing history
- **Admin dashboard** (protected by an `isAdmin` middleware): full CRUD for books, authors, categories, and users
- **REST API** with Laravel Sanctum for book listing and search

## Tech Stack

Laravel 12 · Blade · Tailwind CSS · MySQL · Laravel Sanctum

## Data Model

`users` · `books` · `authors` · `categories` · `borrows`

## Getting Started

```bash
git clone https://github.com/SAJADDIPURO/e-library-IT.git
cd e-library-IT
composer install && npm install
cp .env.example .env && php artisan key:generate
# configure your database in .env
php artisan migrate --seed
npm run build && php artisan serve
```
