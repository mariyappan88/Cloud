# Cloud

# Laravel CLOUDREVEL Management System

This Laravel project manages customers and their leads, allowing users to create, update, and manage customer information and associated leads.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your/repository.git
   cd repository-name
2. composer install

3. cp .env.example .env

4. php artisan migrate


5. Additional information

Packages installed
"spatie/laravel-permission": "^6.9" => for roles assignment.
"laravel/breeze": "^1.29", => Login & Register

User Login and Registration:

Admin Users : admin1@gm.com	
Regular user : user1@gm.com

Admin user can see the Customer management and Lead management navigations in the top.

Regular users cannot able to visible. They can check in profile. 

Note: When register the user, The username contains ‘admin’ it will take as Admin user otherwise regular user. Added this logic in inside RegisteredUser file.

php artisan permission:create-role admin
php artisan permission:create-role user

php artisan db:seed --class=CustomersTableSeeder
php artisan db:seed --class=LeadsSeeder

php artisan db:seed
