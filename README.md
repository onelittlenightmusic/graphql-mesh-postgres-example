# GraphQL Mesh PostgreSQL simple example 

## TL;DR

```sh
# Run PostgreSQL and GraphQL Mesh on container
docker-compose up -d
```

output
```
yarn run v1.22.4
$ graphql-mesh serve
info: 🕸️ => Serving GraphQL Mesh Playground: http://localhost:4000/graphql
```

Then access to `http://localhost:4000`

![](img/screen.png)

## Architecture

- On Docker container
  - #1 GraphQL Mesh with node.js (port 4000)
  - #2 PostgreSQL (port 5432 mapped to host)

Behavior

- #2 runs and initializes database
- #1 accesses to #2 
