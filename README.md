# Description

backend created using nestjs

## Config

Stripe webhook:

```
http://{domain_name}/api/payment/stripe/webhook
```

for development run stripe cli:

```
stripe listen --forward-to localhost:4000/api/payment/stripe/webhook
```

trigger a event for testing:

```
stripe trigger payment_intent.succeeded
```

## Installation

Install all dependencies

```
yarn install
```

## Setup

Copy .env.example to .env and config according to your needs.

Migrate database:

```bash
npx prisma migrate dev
```

Seed dummy data to database

```
yarn cmd seed
```

## Running:

```bash
# development
yarn start

# watch mode
yarn start:dev

# production mode
yarn start:prod

# watch mode with swc compiler (faster)
yarn start:dev-swc
```

For docker:

```
docker compose up
```

## Api documentation

Swagger: http://{domain_name}/api/docs

## Tech used

- Typescript
- Nest.js
- Prisma
- Postgres
- Socket.io
- Bullmq
- Redis
- etc.
// update 1291
// update 13583
// update 9049
// update 26793
// update 18621
// update 14605
// update 17421
// update 15323
// update 20958
// update 3969
// update 5189
// update feat: setup project structure (NestJS)
// update feat: setup project structure (NestJS)
// update feat: implement user CRUD API
// update feat: create inventory module
// update feat: create inventory module
// update feat: implement user CRUD API
// update fix: inventory stock bug
// update refactor: optimize queries
// update fix: inventory stock bug
// update feat: integrate PostgreSQL with Prisma
// update feat: implement user CRUD API
// update feat: add order management API
// update docs: update API documentation
// update fix: API response formatting issue
// update refactor: optimize queries
// update feat: implement user CRUD API
// update feat: implement validation
// update feat: integrate Redis caching
// update fix: resolve auth issue
