This project is a Book Management CRUD application built using Spring Boot that provides a RESTful API to manage books

### Features
- Add new books
- View details of existing books
- Update book information
- Delete books
- List all books

It uses the H2 temporary database

### To run locally
1. Clone the repository
2. Run the project
3. Go to 'localhost:9090/h2' for h2 console
4. Login using the default user id and password
5. Create table Books
6. Use Postman to add, view, update or delete books

### API Endpoints

1. Create a New Book
   - URL: /addBook
   - Method: POST
   - Request Body:
   ```json
   {
     "title": "Book Title",
     "author": "Author Name"
   }
   ```
   ID parameter is self-created for all books.

2. Retrieve All Books
   - URL: /getAllBooks
   - Method: GET

4. Retrieve a single book by ID
   - URL: /getBookById/{id}
   - Method: GET

5. Update an existing book by ID
   - URL: /updateBookById/{id}
   - Method: POST
   - Request Body:
   ```json
   {
     "title": "Updated Book Title",
     "author": "Updated Author Name"
   }
   ```
   
6. Delete a Book
   - URL: /deleteBookById/{id}
   - Method: DELETE
