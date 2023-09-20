

# gRPC Library System with Ballerina

This project implements a gRPC-based library system using the Ballerina programming language. The system allows two types of users, students, and librarians, to interact with the library for managing books, borrowing them, and returning them.

## Features

### Librarian

- `add_book`: Librarian can create a new book with the following details - title, author_1, optional author_2, location, ISBN, and status. The ISBN for the added book is returned.
- `create_users`: Librarian can create multiple user profiles by streaming user data to the server.
- `update_book`: Librarian can update the details of a specific book.
- `remove_book`: Librarian can remove a book from the library collection and return the updated list of books.

### Student

- `list_available_books`: Students can get a list of all available books in the library.
- `locate_book`: Students can search for a book based on its ISBN and get its location if available.
- `borrow_book`: Students can borrow a book by providing their user ID and the book's ISBN.

## Prerequisites

- [Ballerina](https://ballerina.io/downloads/)
- [Protocol Buffers (protobuf)](https://developers.google.com/protocol-buffers)

## Getting Started

1. Clone this repository:

```bash
git clone https://github.com/Swift420/grpc-library-system.git
cd grpc-library-system
```

2. Start the Ballerina server:
```bash
bal run server
```

3. Start the Ballerina Client:
```bash
bal run client
```

## Protocol Buffers Contract
The gRPC service contract is defined in the dsa2.proto file. You can find the details of the service methods, request, and response message structures there.
 
