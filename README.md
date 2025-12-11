University Library Management System - README
Overview: This is a Flask-based Library Management System designed for university libraries. It allows
librarians and library members to manage books, checkouts, and user accounts.

Features:

For Members:

Register and login with authentication
Search and view books by title, author, publication year, or language
Check out and return books
View borrowing history

For Librarians:

Add, edit, and manage books
Track book availability and checkouts
Manage member accounts
View full check-out history
Optional: generate reports

Common Features:
Role-based access control (Member / Librarian)
User-friendly interface
Flash messages for success/error notifications

Project Structure:
library-assignment/
├── app.py # Main Flask app
├── config.py # Configuration for Flask and database
├── models/
│ └── models.py # SQLAlchemy models
├── routes/
│ ├── auth_routes.py # User authentication routes
│ ├── book_routes.py # Book management routes
│ └── checkout_routes.py # Check-in/out routes
├── templates/ # HTML templates
├── static/ # CSS, JS, images
├── requirements.txt # Python dependencies
└── venv/ # Virtual environment
•
•
•
•
•
•
•
•
•
•
•
•
1
Installation and Setup:
Clone the repository:
git clone cd library-assignment

2. Create and activate a virtual environment:
 ```bash
python3 -m venv venv
source venv/bin/activate # macOS/Linux
venv\Scripts\activate # Windows

Install dependencies:
pip install -r requirements.txt

4. Run the application:
 ```bash
python app.py

Open your browser at:
http://127.0.0.1:5000
**Database:**
- SQLite database (`library.db`) is created automatically on first run.
- Tables:
 - **Users:** id, username, email, password hash, role
 - **Books:** id, title, author, language, publication year, availability
 - **Checkouts:** id, user_id, book_id, checkout_date, return_date
**Usage:**
1. Register as a member or login as librarian
2. Add books (librarian only)
3. Search books and check out (members)
4. Return books and view history
1.
1.
1.
2
**Technologies Used:**
- Python 3.x
- Flask 2.x
- Flask-SQLAlchemy
- Flask-WTF
- HTML/CSS/Bootstrap
- SQLite
**Testing:**
- Ensure the virtual environment is active
- Run tests (if implemented) with `pytest`
**Authors / Team Members:**
- Hamid Malikzada
- Asmaa Musafir
- Sonbol Almas
- Sara Qateh
- Zohal Sarwary
**License:**
This project is for educational purposes.
3
