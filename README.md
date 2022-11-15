# NX NestJS React starter

Bootstrapped, ready-for-production (Mono-)Repository for TypeScript environments using NestJS + React.
This project was generated using [Nx](https://nx.dev).

🔎 **Smart, Extensible Build Framework**

## Project setup / initialization

This project setup was created by executing folling steps

- install nx globally `npm i nx`
- install dependencies `npm install` or `npm i`

### adjust package.json

support linting and testing for all applications at once  
`"test": "npx nx run-many --all --target=test --parallel"`  
`"lint": "nx workspace-lint && npx nx run-many --all --target=lint --parallel"`

add separate run & build scripts for backend and frontend  
`"start:client": "nx run client:serve"`  
`"start:api": "nx run api:serve"`

## Adding capabilities to your workspace

Nx supports many plugins which add capabilities for developing different types of applications and different tools.

These capabilities include generating applications, libraries, etc as well as the devtools to test, and build projects as well.

- [React](https://reactjs.org)
  - `npm install --save-dev @nrwl/react`
- [Nest](https://nestjs.com)
  - `npm install --save-dev @nrwl/nest`
- [Node](https://nodejs.org)
  - `npm install --save-dev @nrwl/node`

There are also many [community plugins](https://nx.dev/community) you could add.

## Generate an application

Run `nx g @nrwl/react:app my-app` to generate an application.

> You can use any of the plugins above to generate applications as well.

When using Nx, you can create multiple applications and libraries in the same workspace.

## Generate a library

Run `nx g @nrwl/react:lib my-lib` to generate a react library.
Run `nx g @nrwl/node:library mylib` to create a new node library.

> You can also use any of the plugins above to generate libraries as well.

Libraries are shareable across libraries and applications. They can be imported from `@nx-nestjs-react-starter/mylib`.

## Development server

Run `nx serve client` for a frontend dev server. Navigate to http://localhost:4200/.
Run `nx serve api` for a backend dev server. Navigate to http://localhost:3333/api.  
The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `nx g @nrwl/react:component my-component --project=my-app` to generate a new component.

## Build

Run `nx build api` or `nx build client` respectively to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `nx test api` or `nx test client` to execute the unit tests via [Jest](https://jestjs.io).

Run `nx affected:test` to execute the unit tests affected by a change.

## Running end-to-end tests

Run `ng e2e client` to execute the end-to-end tests via [Cypress](https://www.cypress.io).

Run `nx affected:e2e` to execute the end-to-end tests affected by a change.

## Understand your workspace

Run `nx dep-graph` to see a diagram of the dependencies of your projects.

## Further help

Visit the [Nx Documentation](https://nx.dev) to learn more.
