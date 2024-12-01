# Games Project

## Overview
This is a simple project designed to learn new concepts and revisit important points about HTTP requests, APIs, data security, web programming best practices, and data access.

In the **front-end**, we use **pure HTML** and **JavaScript** with **Axios** for requests. In the **back-end (API)**, we use **JavaScript** with **Node.js** and libraries such as **Express**, **jsonwebtoken**, and **body-parser**.

This project was built using **Node.js 20**.

---

## Concepts

### **CRUD**
- Implementation of CRUD concepts (*Create, Read, Update, and Delete*) by consuming an API to manage game data.

### **HTTP**
- Use of Axios to simplify HTTP requests and integrate the front-end with the API.

### **Data Handling**
- How to process data before sending it in an HTTP request and handle it on the back-end.

### **Routes**
- Structuring routes for sending and receiving data, and defining the expected data for each route.

### **Security**
- Using **JWT (JSON Web Token)** to ensure the security of sending and receiving sensitive data.

### **Message Interpretation**
- Processing the body of HTTP messages using **body-parser**.

### **LocalStorage**
- Storing access information in browsers, and how to insert and access this data.

---

## Application

### Front-end
- **Technologies**: Developed using **HTML5** and **JavaScript** without CSS.
- Main file: **`index.html`** (located in the **`Consumo_API`** folder).
- Purpose: Focus on learning requests and integration between front-end and API.
- **Code details**:
  - The **HTML** and **JavaScript** code is in the same file.
  - The **Axios** library is included via **CDN**, added at the end of the file, before the `</body>` tag.
  - All functions and requests (CRUD), as well as data processing, are encapsulated within the `<script></script>` tag.

### Back-end
- **Technologies**: Developed using **Node.js** with **Express**.
- Main file: **`index.js`**.
- Purpose: Basic educational API, with all logic implemented in a single file.
- **Libraries used**:
  - **body-parser**: To parse the body of HTTP messages.
  - **jsonwebtoken**: To create authentication tokens.
  - **cors**: To configure API access policies.
  - **express**: To create and manage routes and middleware.
- **Mock data**: The data consumed by the API is defined directly in the file.

---

## Resource Installation

Some resources must be installed locally if you clone the repository and wish to test the application since unnecessary production files were removed to optimize repository size.

### Prerequisites

#### **Node.js**
- If you don’t have **Node.js** installed:
  - Download it directly from the official site: [https://nodejs.org/](https://nodejs.org/).
  - Or use **NVM (Node Version Manager)** to install and manage multiple versions:
    - Install **NVM**: [NVM for Windows](https://github.com/coreybutler/nvm-windows).

#### **Node Modules**
- To run the server, install the required modules in the **APIDeGames** folder:
```bash
    npm install
```

### Project Dependencies
Install the following libraries:
#### **body-parser**
- Required to parse the body content of HTTP requests:
```bash
    npm install --save body-parser
```
#### **cors**
- To configure API access policies:
```bash
    npm install --save cors
```
#### **jsonwebtoken**
To create authentication tokens:
```bash
    npm install --save jsonwebtoken
```


## Running the Server
After installing Node.js and dependencies, run the following command in the project folder:
```bash
    node index.js
```

The server will be running and ready for use.


