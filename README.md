# Laravel Job Portal

A comprehensive job portal built with Laravel 10, featuring a clean and intuitive interface using Laravel Blade templates. This application connects job seekers with employers through a robust and user-friendly platform.

## Features

### For Job Seekers
- Browse and search for available jobs
- Apply to jobs with a simple application process
- Save favorite jobs for later reference
- Track job applications
- Create and manage a professional profile
- Upload and update profile picture
- Reset password functionality

### For Employers
- Post new job listings
- Manage existing job postings
- View and manage job applications
- Edit and update job details
- Delete job listings

### Admin Features
- Comprehensive dashboard
- User management
- Job listing management
- Application tracking
- System monitoring

## Technical Requirements

- PHP >= 8.1
- Composer
- MySQL/MariaDB
- Apache/Nginx web server

## Project Structure

```
├── app/
│   ├── Http/
│   │   ├── Controllers/    # Application controllers
│   │   └── Middleware/     # Custom middleware
├── resources/
│   ├── views/
│   │   ├── admin/         # Admin panel views
│   │   ├── front/         # Frontend views
│   │   └── email/         # Email templates
├── routes/
│   ├── web.php           # Web routes
│   └── api.php           # API routes
└── database/
    └── migrations/       # Database migrations
```

## Installation

1. Clone the repository:
```bash
git clone [repository-url]
cd laravel-job-portal
```

2. Install PHP dependencies:
```bash
composer install
```

3. Create environment file:
```bash
cp .env.example .env
```

4. Generate application key:
```bash
php artisan key:generate
```

5. Configure your database in `.env` file:
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database
DB_USERNAME=your_username
DB_PASSWORD=your_password
```

6. Run database migrations:
```bash
php artisan migrate
```

7. Start the development server:
```bash
php artisan serve
```

## Main Routes

### Public Routes
- `/` - Home page
- `/jobs` - List all jobs
- `/jobs/detail/{id}` - View job details
- `/forgot-password` - Password recovery
- `/reset-password/{token}` - Reset password

### Account Routes
- `/account/register` - User registration
- `/account/login` - User login
- `/account/profile` - User profile
- `/account/create-job` - Create job listing
- `/account/my-jobs` - Manage job listings
- `/account/my-job-applications` - View applications
- `/account/saved-jobs` - View saved jobs

### Admin Routes
- `/admin/dashboard` - Admin dashboard
- `/admin/users` - User management
- `/admin/jobs` - Job management
- `/admin/job-applications` - Application management

## Security Features

- Password hashing using Laravel's built-in security
- CSRF protection
- Input validation
- Role-based access control
- Secure file uploads
- Session management
- XSS protection

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support, please open an issue in the repository or contact the development team.
