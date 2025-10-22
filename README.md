# PostgreSQL + pgAdmin Docker Compose

This project allows you to quickly deploy PostgreSQL and pgAdmin using Docker Compose.

## Requirements

-   Docker
-   Docker Compose

## Usage

1. Copy the `.env.example` file to `.env` and customize the environment variables as needed.
2. Start the services:

```
docker-compose up -d
```

## Environment Variables

-   `POSTGRES_USER` — PostgreSQL username (default: postgres)
-   `POSTGRES_PASSWORD` — PostgreSQL password (default: postgres)
-   `POSTGRES_DB` — database name (default: postgres)
-   `POSTGRES_PORT` — PostgreSQL port (default: 5432)
-   `POSTGRES_VOLUME` — volume name for data (default: db-data)
-   `PGADMIN_DEFAULT_EMAIL` — email for pgAdmin login
-   `PGADMIN_DEFAULT_PASSWORD` — password for pgAdmin login
-   `PGADMIN_PORT` — pgAdmin port (default: 80)

## Access

-   PostgreSQL: `localhost:<POSTGRES_PORT>`
-   pgAdmin: `http://localhost:<PGADMIN_PORT>`
