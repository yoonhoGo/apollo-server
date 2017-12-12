---
title: Apollo Server
sidebar_title: Installing
description: Flexible, community driven, production-ready HTTP GraphQL middleware for Node.js. Supports Express, Connect, Hapi, Koa, and more.
---

Apollo Server works with any GraphQL schema built with [GraphQL.js](https://github.com/graphql/graphql-js), Facebook's reference JavaScript execution library, and you can use Apollo Server with all popular JavaScript HTTP servers, including Express, Connect, Hapi, Koa, Restify, and Lambda.

This server can be queried from any popular GraphQL client, such as [Apollo](http://dev.apollodata.com) or [Relay](https://facebook.github.io/relay) because it supports all of the common semantics for sending GraphQL over HTTP, as [documented on graphql.org](http://graphql.org/learn/serving-over-http/). Apollo Server also supports some small extensions to the protocol, such as sending multiple GraphQL operations in one request. Read more on the [sending requests](/tools/apollo-server/requests.html) page.

<h2 id="selecting-package">Selecting the right package</h2>

Apollo Server is actually a family of npm packages, one for each Node.js HTTP server library.

Pick the one below that suits your needs:

```bash
# Pick the one that matches your server framework
npm install graphql apollo-server-express  # for Express or Connect
npm install graphql apollo-server-hapi
npm install graphql apollo-server-koa
npm install graphql apollo-server-restify
npm install graphql apollo-server-lambda
npm install graphql apollo-server-micro
npm install graphql apollo-server-azure-functions
npm install graphql apollo-server-adonis
```

<h2 id="features">Features</h2>

At the end of the day, Apollo Server is a simple, production-ready solution without too many features. Here's what you can do with it:

- Attach a GraphQL schema to your HTTP server to serve requests
- Attach GraphQL and GraphiQL via separate middlewares, on different routes
- Accept queries via GET or POST
- Support HTTP query batching
- Support Apollo Tracing to get performance information about your server
- Support Apollo Cache Control to inform caching gateways such as Apollo Engine

<h2 id="principles">Principles</h2>

Apollo Server is built with the following principles in mind:

* **By the community, for the community**: Apollo Server's development is driven by the needs of developers using the library.
* **Simplicity**: Keeping things simple, for example supporting a limited set of transports, makes Apollo Server easier to use, easier to contribute to, and more secure.
* **Performance**: Apollo Server is well-tested and production-ready.

Anyone is welcome to contribute to Apollo Server, just read [CONTRIBUTING.md](https://github.com/apollographql/apollo-server/blob/master/CONTRIBUTING.md), take a look at the [issues](https://github.com/apollographql/apollo-server/issues) and make your first PR!