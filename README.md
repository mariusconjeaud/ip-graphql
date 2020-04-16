# Quick Start

## Configure

Add a .env file in root folder and set the following variables :

*.env*

```
NEO4J_URI=bolt://localhost:7687
NEO4J_USER=neo4j
NEO4J_PASSWORD=letmein
GRAPHQL_LISTEN_PORT=4001
```

## Start

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

You will find an example query in [src/query-example.graphql]().

Please note that to make this query work, you do need to provide values for runId and topdownId in the *Query variables* section. It should look like this example :

```json
{
    "runId": "whatever"
    "topdownId": "whatever"
}
```

## Build docker image
You can also directly build Docker image from Dockerfile for deployment.

```
docker build . -t ip-graphql
docker images
```