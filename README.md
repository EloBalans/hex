# Hex

This repository uses [Nx](https://nx.dev) to manage both the backend and the frontend.

- **server-lobby** – NestJS module containing server-side lobby features.
- **web-lobby** – Angular web application.

## Prerequisites

- Node.js 18 or newer
- npm or yarn

## Installation

Install all dependencies at the root of the workspace:

```bash
npm install
```

## Running the NestJS server

`server-lobby` is implemented as a NestJS module. To run a server that uses it, create a NestJS application and import `ServerLobbyModule`. After adding an application or a `serve` target, start it with:

```bash
npx nx serve server-lobby
```

Run unit tests for the module with:

```bash
npx nx test server-lobby
```

## Running the Angular web application

Start the development server:

```bash
npx nx serve web-lobby
```

The application will be available at [http://localhost:4200](http://localhost:4200).

## Building

Build the Angular app for production:

```bash
npx nx build web-lobby
```

Build the NestJS module:

```bash
npx nx build server-lobby
```

## Testing

Run unit tests for all projects:

```bash
npx nx test
```
