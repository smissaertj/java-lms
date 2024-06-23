## Problem Statement: Library Management System

### Overview
You are tasked with developing a simple Library Management System using Object-Oriented Programming principles in Java. This system should manage books, library members, and the borrowing and returning of books. You will implement classes representing books, members, and the library itself. Additionally, you will create a custom exception class to handle specific scenarios that may arise during the operation of the library.

### Requirements

1. **Book Class**
   - Attributes: `title`, `author`, `ISBN`, `isAvailable`
   - Methods: `borrowBook()`, `returnBook()`

2. **Member Class**
   - Attributes: `name`, `memberId`, `borrowedBooks`
   - Methods: `borrowBook(Book book)`, `returnBook(Book book)`

3. **Library Class**
   - Attributes: `books`, `members`
   - Methods: `addBook(Book book)`, `removeBook(Book book)`, `registerMember(Member member)`, `borrowBook(Member member, Book book)`, `returnBook(Member member, Book book)`

4. **Custom Exception Class**
   - Name: `LibraryOperationException`
   - Purpose: To handle specific library operation errors such as trying to borrow a book that is not available or a member trying to borrow more books than allowed.

### Functional Requirements

1. **Add and Remove Books**
   - The library should be able to add new books and remove existing books.

2. **Register Members**
   - The library should be able to register new members.

3. **Borrow and Return Books**
   - Members should be able to borrow available books.
   - Members should be able to return borrowed books.

4. **Handle Errors with Custom Exception**
   - If a member tries to borrow a book that is already borrowed, a `LibraryOperationException` should be thrown with an appropriate message.
   - If a member tries to return a book they did not borrow, a `LibraryOperationException` should be thrown with an appropriate message.

### Additional Guidelines

- Ensure proper encapsulation of attributes.
- Implement constructors, getters, and setters as necessary.
- Use collections (e.g., ArrayList) to manage lists of books and members.
- Implement meaningful toString() methods for displaying information about books and members.
- Ensure the `LibraryOperationException` provides useful information about the error.

### Example Scenario

1. Add several books to the library.
2. Register a few members.
3. Members borrow and return books.
4. Handle any errors using the `LibraryOperationException`.
