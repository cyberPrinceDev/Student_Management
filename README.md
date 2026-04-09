# Student Management System

A simple Laravel application built with the TALL stack and **Filament PHP** to manage students and departments.

## Features
- CRUD for **Departments**.
- CRUD for **Students** with:
  - Form validation (Name, Email, Gender).
  - Relationship with Departments.
  - Search and Sort functionality.
  - Filter by Gender.
  - Bulk Delete actions.

## Requirements
- PHP 8.2+
- Composer
- XAMPP / MySQL

## Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/cyberPrinceDev/student_Management.git
   cd studentManagement
   ```

2. **Install PHP dependencies:**
   ```bash
   composer install
   ```

3. **Install Node.js dependencies:**
   ```bash
   npm install
   ```

4. **Environment Setup:**
   - Copy the `.env.example` file to `.env`:
     ```bash
     cp .env.example .env
     ```
   - Update the `.env` file with your database credentials and other configuration settings.

5. **Generate Application Key:**
   ```bash
   php artisan key:generate
   ```

6. **Database Setup:**
   - Create a database in your MySQL server (via XAMPP or similar).
   - Run the migrations to create the database tables:
     ```bash
     php artisan migrate
     ```
   - (Optional) Seed the database with sample data:
     ```bash
     php artisan db:seed
     ```

7. **Build Assets:**
   ```bash
   npm run build
   ```

8. **Start the Development Server:**
   ```bash
   php artisan serve
   ```

9. **Access the Application:**
   - Open your browser and navigate to `http://localhost:8000`
   - Log in to the Filament admin panel at `http://localhost:8000/admin` (default credentials may be set in seeders or check documentation)

## Usage

- Navigate to the admin panel to manage departments and students.
- Use the Filament interface for CRUD operations.

## Contributing

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Submit a pull request.

