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

For questions or feedback, please contact [support@mail.com](mailto:benardopeter4@gmail.com)
