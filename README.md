Absolutely — here is the **plain copy-paste version**. You can copy everything inside the code block directly into your `README.md` file.

```markdown
# Backend Node.js Assignment 5

This project is a simple Express.js server demonstrating basic routes, dynamic route parameters, multiple route parameters, query parameters, and request-response logging middleware.

## Technologies Used

- Node.js
- Express.js
- JavaScript
- npm

## Project Structure

Backend-Nodejs-Assignment5/
│
├── server.js
├── package.json
├── package-lock.json
└── README.md

## Steps to Run the Server

### 1. Clone the repository

```bash
git clone https://github.com/stutisaxena44/Backend-Nodejs-Assignment5.git
```

### 2. Navigate to the project folder

```bash
cd Backend-Nodejs-Assignment5
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the server

```bash
node server.js
```

The server will run at:

http://localhost:3000

You can test the routes using a browser or Postman.

---

# Routes

## 1. Home Route

**Method:** GET

**Endpoint:**

```
/
```

**URL:**

```
http://localhost:3000/
```

**Description:**

Displays a welcome message on the home page.

**Sample Output:**

```
Welcome to Home Page
```

---

## 2. About Route

**Method:** GET

**Endpoint:**

```
/about
```

**URL:**

```
http://localhost:3000/about
```

**Description:**

Displays the About page message.

**Sample Output:**

```
This is About Page
```

---

## 3. Contact Route

**Method:** GET

**Endpoint:**

```
/contact
```

**URL:**

```
http://localhost:3000/contact
```

**Description:**

Displays the Contact page message.

**Sample Output:**

```
This is Contact Page
```

---

## 4. Dynamic User Route

**Method:** GET

**Endpoint:**

```
/user/:name
```

**Description:**

Uses a dynamic route parameter to accept a user's name from the URL.

### Example

Request:

```
GET /user/john
```

URL:

```
http://localhost:3000/user/john
```

**Sample Output:**

```
Hello john
```

Another example:

```
GET /user/Stuti
```

Output:

```
Hello Stuti
```

---

## 5. Multiple Route Parameters

**Method:** GET

**Endpoint:**

```
/product/:id/:category
```

**Description:**

Accepts two dynamic parameters from the URL:

- `id` - Product ID
- `category` - Product category

### Example

Request:

```
GET /product/101/electronics
```

URL:

```
http://localhost:3000/product/101/electronics
```

**Sample Output:**

```
Product ID: 101, Category: electronics
```

---

## 6. Query Parameters

**Method:** GET

**Endpoint:**

```
/search
```

**Description:**

Reads `name` and `role` from query parameters using `req.query`.

### Example

Request:

```
GET /search?name=john&role=developer
```

URL:

```
http://localhost:3000/search?name=john&role=developer
```

**Sample Output:**

```
Name: john, Role: developer
```

Another example:

```
/search?name=Stuti&role=student
```

Output:

```
Name: Stuti, Role: student
```

---

# Request-Response Logging

The application uses Express middleware to display the HTTP request method and URL in the terminal for every incoming request.

For example, if the following routes are accessed:

```
GET /about
GET /user/john
GET /search?name=john&role=developer
```

The terminal displays:

```
GET /about
GET /user/john
GET /search?name=john&role=developer
```

This middleware demonstrates how Express handles incoming requests before passing them to the appropriate route.

---

# API Summary

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/` | Displays the Home Page |
| GET | `/about` | Displays the About Page |
| GET | `/contact` | Displays the Contact Page |
| GET | `/user/:name` | Displays a greeting using the user's name |
| GET | `/product/:id/:category` | Displays product ID and category |
| GET | `/search?name=&role=` | Displays the supplied name and role |

---

# Sample Outputs

### Home

```
Welcome to Home Page
```

### About

```
This is About Page
```

### Contact

```
This is Contact Page
```

### User

Request:

```
GET /user/john
```

Response:

```
Hello john
```

### Product

Request:

```
GET /product/101/electronics
```

Response:

```
Product ID: 101, Category: electronics
```

### Search

Request:

```
GET /search?name=john&role=developer
```

Response:

```
Name: john, Role: developer
```

---

# Assignment Requirements Covered

This project demonstrates:

- Basic Express routes
- Dynamic route parameters
- Multiple route parameters
- Query parameters
- Request method and URL logging
- Request-response handling
- Express middleware

---

## Author

Stuti Saxena
```
