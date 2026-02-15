# NVim db Demo

This repository is a demo of using NVim to connect to and manage a database.

## Setup

### Database Setup with Docker

This project includes a `docker-compose.yml` file that sets up a PostgreSQL database.

### Prerequisites

- Docker and Docker Compose installed on your system

### Starting the Database

Start the PostgreSQL container:

```bash
docker-compose up -d
```

Verify the database is running:

```bash
docker-compose ps
```

### Database Credentials

- **Host:** `localhost`
- **Port:** `5432`
- **Username:** `dbuser`
- **Password:** `dbpassword`
- **Database:** `appdb`

### Connecting to the Database

You can connect using any PostgreSQL client:

```bash
psql -h localhost -U dbuser -d appdb
```

When prompted, enter the password: `dbpassword`

### Stopping the Database

```bash
docker-compose down
```

To also remove the database volume:

```bash
docker-compose down -v
```
