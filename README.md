# Prisma + PNPM workspace

Sample project to begin a simple [Node.js](https://nodejs.org/) application with
[Prisma](https://www.prisma.io/) and a [PNPM](https://pnpm.io/) monorepo.

## TypeScript

This template is set up to get started with
[TypeScript](https://www.typescriptlang.org/). However, if you need JS only, you
can rename the `.ts` to `.js`, remove the types, and remove `tsconfig.json`.
Alternatively, you could keep `tsconfig.json` for better type hints.

## Database

### Provider

The project is set up to work with a `PostgreSQL` database. If you would like to
change that, head to the `schema.prisma` and change it.

### Connect

At the root of this project, next to your `package.json`,  create an `.env`
file. Insert your database environment variables, they will automatically get
deployed. Do not commit this file.

```
DATABASE_URL=postgres://user:password@host:port/db_name
```

## Generate

Run `pnpm -r generate` to run `pnpx prisma generate` in your sub projects.
