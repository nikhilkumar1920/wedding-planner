# Wedding Planner System

A web-based wedding planning system that helps manage decorations, catering, music, and venue bookings.

## Prerequisites

- XAMPP (Apache and MySQL)
- Web Browser (Chrome/Firefox/Edge)
- VS Code (optional, for development)

## Installation Steps

1. **Install XAMPP**
   - Download XAMPP from [https://www.apachefriends.org/download.html](https://www.apachefriends.org/download.html)
   - Install it in the default location (usually C:\xampp)

2. **Copy Project Files**
   - Copy the entire "wedding-planner" folder to: `C:\xampp\htdocs\`
   - The final path should be: `C:\xampp\htdocs\wedding-planner\`

3. **Start XAMPP Services**
   - Open XAMPP Control Panel
   - Click "Start" button next to Apache
   - Click "Start" button next to MySQL
   - Both services should show green background when running

4. **Import Database**
   - Open your browser and go to: [http://localhost/phpmyadmin](http://localhost/phpmyadmin)
   - Click "New" on the left sidebar
   - Create a database named "wedding"
   - Click on the "wedding" database
   - Click "Import" tab at the top
   - Click "Choose File" and select the `wedding.sql` file from the project folder
   - Click "Go" at the bottom to import the database

5. **Access the Website**
   - Open your web browser
   - Go to: [http://localhost/wedding-planner/](http://localhost/wedding-planner/)
   - The wedding planner website should now be visible

## Default Login Credentials

- **Admin Login:**
  - Username: admin
  - Password: admin

## Features

- Wedding decoration management
- Catering service management
- Music/DJ booking
- Venue selection and booking
- User registration and profile management
- Booking management system
- Admin dashboard

## Project Structure

```
wedding-planner/
├── action.php          # Database connection and actions
├── index.php          # Main entry point
├── decoration.php     # Decoration management
├── catering.php      # Catering management
├── music.php         # Music/DJ management
├── venue.php         # Venue management
├── wedding.sql       # Database schema and initial data
└── assets/           # CSS, JS, and image files
```

## Troubleshooting

1. **Cannot access phpMyAdmin:**
   - Make sure both Apache and MySQL are running in XAMPP
   - Check if port 80 and 3306 are not being used by other applications

2. **Database connection fails:**
   - Verify MySQL is running
   - Check database credentials in `action.php`
   - Make sure the "wedding" database exists

3. **Page not found error:**
   - Verify the project folder is in the correct location
   - Check if Apache is running
   - Try accessing through `localhost` instead of IP address

## Development

For developers who want to modify the project:

1. Open the project in VS Code
2. Install PHP extensions in VS Code
3. Use XAMPP for testing
4. Database can be managed through phpMyAdmin or VS Code MySQL extension
