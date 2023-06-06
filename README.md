# Project with a PostgreSQL database

## Description
This project is a simple example of how to use a PostgreSQL database with Python. It uses the psycopg2 library to connect to the database and execute queries.

## Installation
To install the project, you need to have a PostgreSQL database running. You can install the required Python libraries with the following command:
```bash
poetry install
```
To run PostgreSQL in a Docker container, you can use the following command:
```bash
docker run -p 5432:5432 -e POSTGRES_PASSWORD=password postgres
```

## Usage
To run project you need to change `.env.example` to `.env` and fill in the required values. Then you can run the project with the following command:
```bash
poetry run python manage.py migrate
```
This will create the required tables in the database. Then you can run the following command to start the application:
```bash
poetry run python manage.py runserver
```

## Commands
For generate teachers you can use the following command:
```bash
poetry run python manage.py generate_teachers
```