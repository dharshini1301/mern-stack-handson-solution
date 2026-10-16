# Activity 1: How the Internet Works 
Students simulate the interaction between a browser, server, and database to understand how requests are processed and responses are returned
#
# Activity 1: How the Internet Works

## 1. Aim

To understand how a browser, server, and database interact to process requests and return responses through a practical simulation.

## 2. Introduction

The Internet allows computers and devices to communicate with each other. When a user visits a website, the browser sends a request to a web server. The server processes the request and communicates with a database when information is required. The server then returns a response, which the browser displays to the user.

The three main components are:

- **Browser (Frontend):** The application used by the user to access a website.
- **Server (Backend):** Receives requests, processes logic, and communicates with the database.
- **Database:** Stores and retrieves information such as user details, products, and posts.

## 3. Working Principle

The communication follows these steps:

1. The user opens a website or performs an action in the browser.
2. The browser sends an HTTP request to the server.
3. The server receives and processes the request.
4. The server queries the database for the required information.
5. The database returns the requested data to the server.
6. The server sends an HTTP response to the browser.
7. The browser displays the received information to the user.

## 4. Flowchart

```text
           +-------------+
           |    START    |
           +-------------+
                  |
                  v
       +----------------------+
       | Browser sends request|
       +----------------------+
                  |
                  v
       +----------------------+
       | Server receives and  |
       | processes request    |
       +----------------------+
                  |
                  v
       +----------------------+
       | Server requests data  |
       | from the database    |
       +----------------------+
                  |
                  v
       +----------------------+
       | Database retrieves   |
       | and returns data     |
       +----------------------+
                  |
                  v
       +----------------------+
       | Server sends response|
       | to the browser       |
       +----------------------+
                  |
                  v
       +----------------------+
       | Browser displays     |
       | the response         |
       +----------------------+
                  |
                  v
           +-------------+
           |     END     |
           +-------------+
```

## 5. Practical Implementation Using Python

The following program simulates the interaction between a browser, server, and database.

### Source Code

Save the code in a file named `activity1.py`.

```python
# Activity 1: How the Internet Works

# Simulating the browser
def browser():
    print("Browser: Sending request to server...")
    response = server()
    print("Browser: Response received.")
    print("Browser: Displaying:", response)


# Simulating the server
def server():
    print("Server: Request received.")
    print("Server: Requesting data from database...")

    data = database()

    print("Server: Sending response to browser...")
    return data


# Simulating the database
def database():
    print("Database: Retrieving data...")
    return "Welcome to the MERN Stack!"


# Start the simulation
browser()
```

## 6. Output

```text
Browser: Sending request to server...
Server: Request received.
Server: Requesting data from database...
Database: Retrieving data...
Server: Sending response to browser...
Browser: Response received.
Browser: Displaying: Welcome to the MERN Stack!
```

## 7. Code Explanation

**Browser function:** Simulates sending a request to the server and displaying the response returned by it.

**Server function:** Receives the request, calls the database function, obtains the data, and returns the response to the browser.

**Database function:** Simulates retrieving stored information and returning it to the server.

**Main function call:** The `browser()` call starts the entire simulation.

**Note:** This is a simplified simulation. It uses Python functions rather than actual HTTP communication or a real database.

## 8. Real-World Example

Consider a user logging into an online shopping website.

- **Browser:** Sends the login request.
- **Server:** Validates the submitted credentials.
- **Database:** Provides the stored user information needed for verification.
- **Response:** The server returns a success or failure response, and the browser displays the appropriate result.

In a real application, passwords should be securely hashed, and authentication should be handled using appropriate security practices.

## 9. Connection to the MERN Stack

The MERN stack consists of four technologies:

| Technology | Purpose |
|---|---|
| MongoDB | Stores application data |
| Express.js | Handles backend routes and requests |
| React.js | Builds the user interface |
| Node.js | Runs JavaScript on the server |

In a MERN application, React sends requests to a Node.js and Express.js backend. The backend interacts with MongoDB and returns data to React.

## 10. Result

Successfully simulated the communication between a browser, server, and database using Python. The request-processing flow, database interaction, and response delivery were understood through a flowchart, source code, and output.
