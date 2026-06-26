# Library Management System

![C++](https://img.shields.io/badge/language-C++-blue.svg)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux-lightgrey.svg)
![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)

A console-based Library Management System built in C++ using Object-Oriented Programming principles.

The project allows a library admin to manage books, register users, borrow and return books, search books by ISBN, and save data in text files.

## Features

- Add, remove, list, and search books
- Register and list users
- Prevent duplicate ISBN entries
- Prevent duplicate user IDs
- Borrow and return books
- Apply borrowing limits for students and faculty
- Track multiple copies of the same book
- Prevent the same user from borrowing the same book twice
- Store data in text files
- Automatically create required data files if they do not exist

## Library Menu

Below is a sample of the interactive menu:

![1782491465096](image/README/1782491465096.png)

## Project Files

- `main.cpp` - starts the program
- `Book.h` / `Book.cpp` - define the Book class
- `User.h` / `User.cpp` - define the User class
- `LibraryManager.h` / `LibraryManager.cpp` - contain the main library logic
- `books.txt` - stores book records in `title|author|isbn|copies` format
- `users.txt` - stores user records in `name|id|userType|borrowLimit` format
- `borrowed.txt` - stores borrowed book records in `userId isbn` format

## Installation and Usage

### 1. Clone the Repository

```bash
git clone https://github.com/Lakshya-coder-1418/Library-Management-System.git
cd Library-Management-System
```

### 2. Compile the Project

```bash
g++ main.cpp Book.cpp User.cpp LibraryManager.cpp -o library
```

### 3. Run the Program

On Windows PowerShell:

```powershell
.\library.exe
```

On Linux or macOS:

```bash
./library
```

## Menu Options

```text
1. Add Book
2. Remove Book
3. Add User
4. List Books
5. List Users
6. Search Book
7. Borrow Book
8. Return Book
0. Exit
```

## Important Notes

- The program saves data when you choose `0. Exit`.
- Keep `books.txt`, `users.txt`, and `borrowed.txt` in the same folder as the executable.
- Do not upload generated `.exe` files to GitHub. They are ignored through `.gitignore`.
- This is a beginner-friendly console project intended for learning C++ OOP, file handling, and basic project structure.

## Learning Goals

This project demonstrates:

- Classes and objects
- Header and source file separation
- Vectors
- File input/output
- Basic validation
- Menu-driven console applications
- Simple data persistence
