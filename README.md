# Quick Start

Install dependencies:

```
npm install
```

Start the GraphQL service:

```
npm start
```

This will start the GraphQL service (by default on localhost:4001) where you can issue GraphQL requests or access GraphQL Playground in the browser:

![GraphQL Playground](img/graphql-playground.png)

## Configure

Add a .env file in root folder and set the following variables :

*.env*

```
NEO4J_URI=bolt://localhost:7687
NEO4J_USER=neo4j
NEO4J_PASSWORD=letmein
```