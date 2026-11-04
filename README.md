# ANAO HRMS

A health and community records management system built with Laravel, Livewire and Flux UI. It covers citizen and household records, clinical workflows, pharmacy and lab/radiology orders, assistance requests, and community surveys.

## Features

- **Citizens & households** – citizen profiles, ID documents, households, barangays
- **Clinical** – appointments, triage, consultations, admissions, wards and beds, nursing notes
- **Diagnostics** – lab orders and tests, radiology orders, imaging exams
- **Pharmacy** – medicines, prescriptions, dispensing, stock movements
- **Social services** – assistance types and requests, field visits
- **Surveys** – questions, responses and answers
- **Authentication** – Laravel Fortify

## Tech stack

- PHP 8.3+, Laravel 13
- Livewire 4, Flux UI 2
- Tailwind CSS 4, Vite
- Pest for testing, Pint and Larastan for code quality
- SQLite by default

## Getting started

```bash
git clone https://github.com/Sephy57/anao-hrms.git
cd anao-hrms

composer install
npm install

cp .env.example .env
php artisan key:generate
php artisan migrate

npm run dev
php artisan serve
```

A reference SQL schema is available at `database/anao-hrms.sql`.

## Testing and code quality

```bash
php artisan test        # Pest test suite
vendor/bin/pint         # code style
vendor/bin/phpstan      # static analysis
```

## License

MIT
