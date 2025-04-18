# PHP Installation Guide

## Required Software

- **PHP**: The PHP language interpreter
- **Composer**: PHP package manager
- **Web Server**: Apache, Nginx, or built-in PHP server
- **Database**: MySQL, PostgreSQL, SQLite (common options)
- **VS Code**: With PHP extensions (recommended)
- **PHPStorm**: Dedicated PHP IDE (alternative)
- **Xdebug**: Debugging extension for PHP

## File Extensions

- `.php` - PHP code files
- `.phtml` - PHP/HTML template files
- `.phps` - PHP source file with syntax highlighting
- `.phar` - PHP archive (executable)
- `.inc` - PHP include files
- `.module` - PHP module files (mainly in CMS like Drupal)
- `.view` - PHP view files
- `.composer.json` - Composer package configuration
- `.composer.lock` - Composer dependency lock file
- `.phpunit.xml` - PHPUnit configuration
- `.htaccess` - Apache configuration file

## Package Management

```bash
# Install Composer
curl -sS https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer

# Create a new project
composer create-project vendor/package-name project-name

# Initialize a new project
composer init

# Install dependencies
composer install

# Add a package
composer require vendor/package-name

# Add a development package
composer require --dev vendor/package-name

# Update packages
composer update

# Remove a package
composer remove vendor/package-name

# Show installed packages
composer show
```

## Running PHP Programs

```bash
# Run a PHP script
php script.php

# Run with specific PHP configuration
php -c /path/to/php.ini script.php

# Run built-in web server
php -S localhost:8000

# Run with a specific document root
php -S localhost:8000 -t public/

# Check syntax without running
php -l script.php

# Run with error reporting
php -d error_reporting=E_ALL script.php

# Run as a web application
# Place files in web server directory and access via browser
# e.g., http://localhost/script.php
```

## Common Libraries

- **Web Frameworks**: Laravel, Symfony, CodeIgniter, Yii, Slim, CakePHP
- **API**: Lumen, API Platform, Symfony API
- **CMS**: WordPress, Drupal, Joomla
- **Testing**: PHPUnit, Behat, Codeception
- **Database ORM**: Doctrine, Eloquent
- **Template Engines**: Blade, Twig, Smarty
- **HTTP Clients**: Guzzle, Symfony HTTP Client
- **Authentication**: OAuth, JWT, Laravel Passport
- **File Handling**: Flysystem, Intervention Image
- **Queue Processing**: Laravel Queue, PHP-Queue
- **PDF Generation**: TCPDF, mPDF, DomPDF
- **Excel/CSV**: PhpSpreadsheet, CSV
- **Validation**: Symfony Validator, Respect\Validation
