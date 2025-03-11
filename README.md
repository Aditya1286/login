# Login System

A secure authentication system built with HTML, Tailwind CSS, and PHP that provides user registration and login functionality.

## Features

- **User Registration**: New users can create accounts with secure password storage
- **Login Authentication**: Secure verification of user credentials
- **Password Hashing**: Passwords are securely hashed for storage
- **Responsive Design**: Built with Tailwind CSS for a seamless experience across devices
- **Form Validation**: Client-side and server-side validation for data integrity
- **Session Management**: Keeps users logged in across pages
- **Security Features**: Protection against common vulnerabilities (SQL injection, XSS)

## Tech Stack

- **Frontend**: HTML, Tailwind CSS
- **Backend**: PHP
- **Database**: MySQL (recommended)

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/Aditya1286/login.git
   ```

2. Configure your web server (Apache/Nginx) to point to the project directory

3. Import the database schema (see `database/schema.sql`)

4. Configure the database connection in `config.php`:
   ```php
   // Update with your database credentials
   $host = "localhost";
   $username = "root";
   $password = "";
   $database = "login_db";
   ```

5. Access the application through your web browser

## Usage

### Registration
1. Navigate to the signup page
2. Enter required information (username, email, password)
3. Submit the form to create your account

### Login
1. Navigate to the signin page
2. Enter your credentials
3. Upon successful authentication, you'll be redirected to the dashboard

## Security Considerations

- All passwords are hashed using PHP's password_hash() function
- Input validation is performed on both client and server sides
- Prepared statements are used to prevent SQL injection attacks
- CSRF protection is implemented on forms

## Directory Structure

```
├── config/
│   └── config.php         # Database configuration
├── css/
│   └── style.css          # Compiled Tailwind CSS
├── js/
│   └── validation.js      # Client-side form validation
├── includes/
│   ├── functions.php      # Helper functions
│   ├── header.php         # Page header template
│   └── footer.php         # Page footer template
├── signin.php             # Login page
├── signup.php             # Registration page
├── logout.php             # Logout script
├── dashboard.php          # User dashboard after login
└── index.php              # Main entry point
```

## Future Enhancements

- Password reset functionality
- Email verification
- Two-factor authentication
- Remember me functionality
- User profile management

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

Aditya - [GitHub Profile](https://github.com/Aditya1286)

Project Link: [https://github.com/Aditya1286/login.git](https://github.com/Aditya1286/login.git)
