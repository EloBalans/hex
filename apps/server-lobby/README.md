# server-lobby

NestJS module providing lobby functionality.

## Setup

Install dependencies in the repository root:

```bash
npm install
```

## Building

```bash
npx nx build server-lobby
```

## Running unit tests

```bash
npx nx test server-lobby
```

## Using in a NestJS server

This library exports `ServerLobbyModule`. To run a NestJS server that uses it, create an application and import the module:

```ts
import { NestFactory } from '@nestjs/core';
import { ServerLobbyModule } from '@hex/source/server-lobby';

async function bootstrap() {
  const app = await NestFactory.create(ServerLobbyModule);
  await app.listen(3333);
}
bootstrap();
```
