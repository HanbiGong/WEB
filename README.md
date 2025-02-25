#Library Book Borrowing API

This is a simple Node.js Express server that allows users to borrow and return books, check overdue status, and view API documentation using Swagger.

##Features

```bash
- Borrow a book
- Return a book
- Check if a book is overdue
- Serve API documentation with Swagger
- Basic frontend UI

##Installation

Clone the repository:

git clone <repository-url>
cd WEB

Install dependencies:

npm install

Start the server:

node server.js

The server will run at http://localhost:3000.

Access the API documentation at:

http://localhost:3000/api-docs

API Endpoints

Borrow a Book

URL: /borrow

Method: POST

Request Body:

{
  "username": "testUser"
}

Response:

{
  "message": "Book successfully borrowed! Enjoy your reading.",
  "user": {
    "username": "testUser",
    "borrowedAnything": true,
    "borrowedDate": "2024-02-25T12:34:56.789Z"
  }
}

Return a Book

URL: /return

Method: POST

Request Body:

{
  "username": "testUser"
}

Response:

{
  "message": "Book returned! Thank you, hope you enjoyed it!",
  "user": {
    "username": "testUser",
    "borrowedAnything": false,
    "borrowedDate": null
  }
}

Check Overdue Books

URL: /check-late?username=testUser

Method: GET

Response:

{
  "message": "No overdue books found.",
  "lateDays": 5
}

Project Structure

WEB/
├── public/               # Static files (e.g., images, styles)
├── server.js            # Main server file
├── swagger.yaml         # API documentation
├── package.json         # Dependencies and scripts
└── README.md            # Project documentation

Dependencies

Express

Body-parser

Luxon (for date handling)

Swagger-UI-Express

YAMLJS

License

This project is licensed under the MIT License.


