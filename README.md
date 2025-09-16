SQLite CRUD Console Application
https://img.shields.io/badge/Python-3.6+-blue.svg
https://img.shields.io/badge/SQLite-3.x-green.svg

A Python console application for performing CRUD (Create, Read, Update, Delete) operations on an SQLite database with a simple menu-driven interface.

Features
🗃️ Automatic database and table creation

➕ Add new records with complete details

👁️ View all records in readable format

✏️ Update individual fields (name, age, gender, etc.)

❌ Delete records by ID

🔄 Interactive console menu

🛠️ Object-oriented design with Database class

Installation
bash
# Clone the repository
git clone https://github.com/Dhivya-ramasamy123/SQLITE_CRUD.git

# No additional dependencies needed (uses built-in sqlite3)
Usage
Run the application:

bash
python sqlite_crud.py
Follow the menu prompts:

text
1) Insert Record
2) Fetch Record
3) Update Record
4) Delete Record

Please Enter Your Operation:
Database Schema
The application automatically creates this table structure:

sql
CREATE TABLE IF NOT EXISTS datas(
    id INTEGER PRIMARY KEY,
    name TEXT NOT NULL,
    age INTEGER NOT NULL,
    gender TEXT NOT NULL,
    address TEXT NOT NULL,
    contact TEXT NOT NULL,
    mail TEXT NOT NULL
)
Sample Operations
Inserting a Record
text
Enter Your Name: John Doe
Enter Your Age: 30
Enter Your Gender: Male
Enter Your Address: 123 Main St
Enter Your Contact: 555-1234
Enter Your Mail: john@example.com
Record Added Successfully
Viewing Records
text
List of Records
---------------
(1, 'John Doe', 30, 'Male', '123 Main St', '555-1234', 'john@example.com')
Updating a Record
text
1. Name
2. Age
3. Gender
4. Address
5. Contact
6. Mail

Which field you want to update?: 2
Enter Your ID: 1
Enter Your Age: 31
Update Successfully
Deleting a Record
text
Enter Your ID: 1
Record Deleted Successfully
Requirements
Python 3.6+

No external dependencies (uses built-in sqlite3 module)

Project Structure
text
sqlite-crud-app/
├── sqlite_crud.py     # Main application file
├── README.md          # Documentation
└── Sqlitedatabase.db  # Database file (auto-created)
License
MIT License - Free to use and modify

Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.