# Book-Management-System
a user-friendly Book Management System application that simplifies and automates the management of a library's book inventory.

Detailed Report on Book Management System Code
Introduction
This document provides an in-depth analysis of a Python application that manages book information using
SQLite for data storage and Tkinter for the graphical user interface. The system enables users to add,
search, and display books with features to manage a library database effectively.
1. Database Setup with SQLite
The application begins by creating a local SQLite database named 'library.db' to store book information. The
database structure includes a 'books' table with columns for ID, title, author, and genre. The table schema
ensures all fields are required, and the ID field is set to auto-increment for each new entry.
2. Importing Tkinter and Setting Up the Main Window
The main application window is created using Tkinter, a Python library for GUI applications. Custom fonts are
defined to enhance readability, and various UI elements, such as buttons and entry fields, are arranged using
Tkinter's grid layout.
3. Add Book Section
The 'Add Book' section allows users to enter book details (title, author, genre) and save them to the
database. The section includes labels, entry fields, and a button to submit the book information to the
database. A confirmation message appears upon successful entry.
4. `add_book` Function
The `add_book` function retrieves user input from the entry fields and saves the book details to the database.
If any field is empty, an error message appears. Otherwise, the book is added to the database, and a
success message is shown. The function also clears the entry fields after a successful addition.
5. Search Book Section and `search_book` Function
The 'Search Book' section allows users to find books by title or author. The section includes a search box and
a button that triggers the `search_book` function, which displays matching results in the list box. The
`search_book` function uses a partial match to find books by title or author and displays them if any records
match.
6. Display All Books Section
The 'Display All Books' button lists all books stored in the database by calling the `display_all_books`
function. This function retrieves all records from the database and shows them in the list box for easy viewing
of all entries.
