````markdown
# FastAPI Auth Demo

This is a simple FastAPI project demonstrating basic authentication using JWT (JSON Web Tokens), SQLite, and SQLAlchemy.

## Features

- **User Registration**: Users can create an account with a username and password.
- **Login**: Users can authenticate and receive a JWT.
- **Secure Routes**: Only authenticated users can access protected endpoints.
- **SQLite Database**: Lightweight database for storing user credentials.

## 🚀 Quick Start

Clone the repository and install dependencies.

### 1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/fastapi-auth-demo.git
cd fastapi-auth-demo
````

### 2. Install dependencies:

```bash
pip install -r requirements.txt
```

### 3. Initialize the database:

```bash
python init_db.py
```

### 4. Run the server:

```bash
uvicorn main:app --reload
```

### 5. Access the Swagger docs at:

[http://localhost:8000/docs](http://localhost:8000/docs)

## 📁 Project Structure

```
.
├── main.py          # API Endpoints: Register, Login, Secure Route
├── models.py        # SQLAlchemy Models
├── database.py      # Database connection and session management
├── security.py      # JWT creation, password hashing and verification
├── init_db.py       # Initializes the database
├── requirements.txt # Project dependencies
```

## 🔒 Authentication Flow

* **/register**: Endpoint to create a new user.
* **/token**: Login and get a JWT token.
* **/secure-data**: A protected route requiring a valid JWT token.

## 🛠️ Technologies Used

* **FastAPI**: For building the API.
* **SQLAlchemy**: ORM for interacting with SQLite.
* **SQLite**: Lightweight database for user credentials.
* **PassLib**: For password hashing.
* **JWT (JSON Web Token)**: For authentication.

## 📄 License

MIT License. See the LICENSE file for more details.
