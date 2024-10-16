# Book Management API

This is a simple Book Management API built using FastAPI, SQLAlchemy, and Docker. The app allows you to manage books and authors in a PostgreSQL database.
## Screenshots

![App Screenshot](https://imgur.com/OFw5gNf.png)
![App Screenshot2](https://imgur.com/bZgVTPn.png)

## Features

- Add and manage books with title, rating, and author information.
- Add and manage authors with name and age.
- Fetch a list of books.
- Containerized using Docker for easy deployment.


## Requirements

- Docker
- Docker Compose
## Tech Stack

**FastAPI:** Web framework for building APIs with Python 3.9

**SQLAlchemy:** ORM(Object-Relational Mapping) for interacting with the database

**PostgreSQL:** Database for storing books and authors data

**Alembic:** For database migrations

**Docker:** Containerization for easier development and deployment.

**Uvicorn:** ASGI server to run the FastAPI app.

**Pydantic:** Data validation and parsing.


## Installation

1. Clone the Repo

```bash
  git clone https://github.com/chemoiko/dockerfastapi-postgres-bookmanagement-api.git


```
2. Environment Variables

```bash
DATABASE_URL=postgresql://<username>:<password>@<db_host>:<db_port>/<db_name>


```

3. Build and Run with Docker

```bash
  docker-compose up --build



```

4. API Endpoints
    
- GET /: A simple welcome message.
- POST /add-author/: Add a new author (name and age).
- POST /add-book/: Add a new book (title, rating, and author).
- GET /books/: Fetch a list of all books.

5. Database Migrations

  ```bash
docker-compose run app alembic revision --autogenerate -m "New Migration"



```

6. Apply the migration:

  ```bash
  docker-compose run app alembic upgrade head



```
## Usage/Examples

```javascript
import Component from 'my-project'

function App() {
  return <Component />
}
```

## Usage

1. The home page contains all the products. You can add the products to your cart by clicking on the Add To Cart button and you will see the number of items in the cart icon update dynamically.
<img src="https://imgur.com/dkLzsUy">

2. Click on the cart icon in nav to see all the items you added to cart.

3. The up and down arrow buttons can be used to change the quantity and the prices and total will change automatically.

4. The user can confirm order using the Checkout button.
5. If the user is logged in, he will not be asked to fill in his name and email.
6. The user will fill in the shipping details and click continue to payment.
<img src="https://imgur.com/undefined">
7. A guest user can also order items through cookies.

_Reference Dennis Ivy YouTube tutorial_
