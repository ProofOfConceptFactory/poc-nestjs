Hello from NestJS!👋
========================

The "Hello from NestJS!👋" application is just a starter to show a minimalist NestJS app.

Requirements
------------

* [Docker Desktop][1]

Installation
------------

Clone this repository:

```console
https://github.com/ProofOfConceptFactory/poc-nestjs
```

Go on the project root folder:

```console
cd poc-nestjs/
```

Execute this command to launch docker container:

```console
docker compose -f docker/compose.yaml up -d --build
```

Install JavaScript dependencies:

```console
docker compose -f docker/compose.yaml exec node pnpm install
```

Usage
-----

There's no need to configure anything before running the application. There are
2 different ways of running this application depending on your needs:

**Option 1. Run the application in dev mode**

Start the application using the dev server:

```console
docker compose -f docker/compose.yaml exec node pnpm start:dev
```

Then access the application in your browser at the given URL (<http://localhost:3000> by default).

**Option 2. Run the application in prod mode**

```console
docker compose -f docker/compose.yaml exec node pnpm start:prod
```
You can check everything is OK by opening the same URL as dev and navigate on your application.

Tests
-----

Execute this command to run tests:

```console
docker compose -f docker/compose.yaml exec node pnpm test
```

Execute this command to run tests for e2e:

```console
docker compose -f docker/compose.yaml exec node pnpm test:e2e
```

[1]: https://www.docker.com/products/docker-desktop/
