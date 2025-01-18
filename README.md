Project Description: Library Management System
This Python-based Library Management System (LMS) is designed to streamline the management of books, students, and transactions. It features a user-friendly graphical interface powered by Tkinter, handles data using CSV files, and incorporates time management functionalities with the datetime module.

Key Features:
Book Management:
Add, view, and manage books in the library.
Search for books by ID, title, or author.
Track the availability and stock of books.

Student Management:
Add and maintain student records.
Keep track of the books borrowed by each student.
Enforce a limit of 3 books per student at any time.
Transaction Management:
Issue books to students with transaction logs including issue dates.
Handle book returns, with automatic penalty calculations for late returns (penalty capped at $50).
Maintain a comprehensive log of all transactions.

Graphical User Interface (GUI):
Easy-to-navigate interface developed with Tkinter.
Dedicated sections for managing books, students, and transactions.
Data Persistence:
Data stored in CSV files (books.csv, students.csv, and logs.csv).
The system automatically loads and saves data when the application starts and exits.

How the System Works:
Book Issue:

Ensures the book is available and the student hasn't exceeded their borrowing limit.
Deducts one copy from the book stock and records the transaction.
Book Return:

Updates book stock upon return.
Removes the book from the student's borrowing list.
Automatically calculates penalties for late returns, with a cap of $50, and records the return transaction.
Search:

Search books or students quickly using the search bar, with results filtered by keyword (ID, title, or author).

Technologies Used:

Python Modules:

tkinter: For building the graphical interface.
csv: For file handling and data storage.
datetime: For managing issue/return dates and calculating penalties.
messagebox: For user feedback and handling errors.
Usage:

Run the Application:
Launch the application by running python library_management.py.

Using the GUI:
Use the search bar to find books or students.
Manage book issues and returns directly from the interface.
View late return penalties where applicable.

Limitations:
The system relies on CSV files for data storage, which may not scale efficiently with large datasets. A migration to a database (e.g., SQLite) would provide better scalability.
Error handling and input validation could be expanded for improved robustness.

Future Enhancements:
Implement a reservation system for books.
Add user authentication to restrict access to librarian functionalities.
Integrate data visualization features for transaction trends and library usage.
Transition from CSV file storage to a more efficient database system to handle larger volumes of data.
