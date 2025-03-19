# Book Reading Management System

A comprehensive web application to track and manage your book reading progress, built with Django, HTML, CSS, and JavaScript.

## Features

- **User Authentication System**: Register, login, and password reset
- **Book Management**: Add, edit, and delete books from your library
- **Reading Progress Tracking**: Track your current page and completion percentage
- **Reading Status**: Categorize books as "To Read", "Currently Reading", "Completed", or "Abandoned"
- **Dashboard**: Get a quick overview of your reading activity
- **Notes & Highlights**: Save important quotes or thoughts while reading
- **Reading Statistics**: View your reading habits and progress over time

## Tech Stack

- **Backend**: Django (Python)
- **Frontend**: HTML, CSS, JavaScript
- **Database**: SQLite (default) / PostgreSQL (recommended for production)

## Installation

### Prerequisites

- Python 3.8+
- pip (Python package manager)

### Setup Instructions

1. Clone the repository:
   ```
   git clone https://github.com/n-cognto/book-tracker.git
   cd book-tracker
   ```

2. Create and activate a virtual environment:
   ```
   python -m venv venv
   
   # On Windows
   venv\Scripts\activate
   
   # On macOS/Linux
   source venv/bin/activate
   ```

3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

4. Set up the database:
   ```
   python manage.py migrate
   ```

5. Create a superuser for the admin panel:
   ```
   python manage.py createsuperuser
   ```

6. Start the development server:
   ```
   python manage.py runserver
   ```

7. Open your browser and navigate to http://127.0.0.1:8000/

## Project Structure

```
book_tracker/
├── book_tracker/       # Main project configuration
├── books/              # Book management app
├── accounts/           # User authentication app
├── templates/          # HTML templates
│   ├── base.html
│   ├── books/
│   └── registration/
└── static/             # Static files (CSS, JavaScript)
    ├── css/
    └── js/
```

## User Guide

### Registration and Login

1. Navigate to the registration page to create an account
2. After registering, you'll be automatically logged in
3. For returning users, use the login page
4. If you forget your password, use the "Forgot Password" link

### Adding Books

1. Click on "Add Book" in the navigation menu
2. Fill in the book details (title, author, page count, etc.)
3. Select the reading status
4. Click "Add Book" to save

### Tracking Reading Progress

1. Go to "My Books" to see your collection
2. For books you're currently reading, click "Update Progress"
3. Enter your current page number and update status if needed
4. The system will automatically calculate your completion percentage

### Using the Dashboard

1. The dashboard provides a quick overview of your reading activity
2. See currently reading books, completion percentages, and reading stats
3. Track your progress toward reading goals

## Development

### Running Tests

```
python manage.py test
```

### Creating New Apps

```
python manage.py startapp appname
```

## Deployment

For production deployment:

1. Update `settings.py` with production settings:
   - Set `DEBUG = False`
   - Update `ALLOWED_HOSTS`
   - Configure a production database (PostgreSQL recommended)

2. Collect static files:
   ```
   python manage.py collectstatic
   ```

3. Set up a production web server (Gunicorn, Nginx, etc.)

## Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature/feature-name`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature/feature-name`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements

- Django documentation
- Bootstrap (if used)
- Any other libraries or resources used

## Contact

For questions or feedback, please contact [your-email@example.com](mailto:your-email@example.com)
