# Running example in docker

Follow README.md, but use the following commands instead whenever applicable

## Getting started

### 1. install dependencies

```bash
docker compose run --rm backend npm install
```

```bash
docker compose run --rm frontend npm install
```

### 2. Create and seed the database (backend)

```bash
docker compose run --rm backend npx prisma migrate dev --name init
```

```bash
docker compose run --rm backend npx prisma db seed
```

### 3. and 4. Start backend and frontend servers

```bash
docker compose up
```