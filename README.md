# Library-Management-System
This is a Flask-based Library Management System designed for university libraries. It allows librarians and
library members to manage books, checkouts, and user accounts.
Features
For Members:
•
•
•
•
Register and login with authentication
Search and view books by title, author, publication year, or language
Check out and return books
View borrowing history
For Librarians:
•
•
•
•
•
Add, edit, and manage books
Track book availability and checkouts
Manage member accounts
View full check-out history
Optional: generate reports
Common Features:
•
•
•
Role-based access control (Member / Librarian)
User-friendly interface
Flash messages for success/error notifications
Project Structure
library-assignment/
├── app.py ├── config.py # Main Flask app
# Configuration for Flask and database
├── models/
│ └── models.py # SQLAlchemy models
├── routes/
│ ├── auth_routes.py # User authentication routes
│ ├── book_routes.py # Book management routes
│ └── checkout_routes.py # Check-in/out routes
├── templates/ # HTML templates
├── static/ # CSS, JS, images
1
├── requirements.txt # Python dependencies
└── venv/ # Virtual environment
Installation and Setup
1.
Clone the repository:
git clone <your-repo-link>
cd library-assignment
1.
Create and activate a virtual environment:
python3 -m venv venv
source venv/bin/activate # macOS/Linux
venv\Scripts\activate # Windows
1.
Install dependencies:
pip install -r requirements.txt
1.
Run the application:
python app.py
1.
Open your browser at:
http://127.0.0.1:5000
Database
•
•
•
•
•
SQLite database is used ( library.db automatically created on first run)
Tables include:
Users: id, username, email, password hash, role
Books: id, title, author, language, publication year, availability
Checkouts: id, user_id, book_id, checkout_date, return_date
2
Usage
1.
2.
3.
4.
Register as a member or login as librarian
Add books (librarian only)
Search books and check out (members)
Return books and view history
Technologies Used
•
•
•
•
•
•
Python 3.x
Flask 2.x
Flask-SQLAlchemy
Flask-WTF
HTML/CSS/Bootstrap
SQLite
Testing
•
•
Ensure the virtual environment is active
Run tests (if implemented) with:
pytest
Authors / Team Members
•
•
•
Member 1
Member 2
Member 3
(Add all group members here)
License
This project is for educational purposes.
3
