# TypeScript Installation Guide

## Required Software

- **Node.js**: JavaScript runtime (required for npm)
- **npm**: Node Package Manager (comes with Node.js)
- **TypeScript Compiler**: Transpiles TypeScript to JavaScript
- **VS Code**: Editor with built-in TypeScript support (recommended)
- **WebStorm**: Alternative IDE with TypeScript support
- **Git**: For version control and package installation

## File Extensions

- `.ts` - TypeScript source files
- `.tsx` - TypeScript files with JSX syntax
- `.d.ts` - TypeScript declaration files
- `.js` - JavaScript files (output from TypeScript)
- `.js.map` - Source map files
- `.json` - JSON configuration files
- `tsconfig.json` - TypeScript compiler configuration
- `package.json` - Project configuration and dependencies
- `package-lock.json` - Dependency lock file
- `.tsbuildinfo` - TypeScript incremental build information
- `.test.ts` - TypeScript test files
- `.spec.ts` - TypeScript specification files

## Package Management

```bash
# Install TypeScript globally
npm install -g typescript

# Initialize a new project
npm init -y

# Initialize TypeScript configuration
npx tsc --init

# Install TypeScript as a dev dependency
npm install --save-dev typescript

# Install type definitions for a library
npm install --save-dev @types/library-name

# Install testing libraries
npm install --save-dev jest ts-jest @types/jest

# Install TypeScript ESLint
npm install --save-dev eslint @typescript-eslint/parser @typescript-eslint/eslint-plugin

# Install development tools
npm install --save-dev ts-node nodemon

# Update packages
npm update
```

## Running TypeScript Programs

```bash
# Compile a TypeScript file
tsc file.ts

# Compile a project using tsconfig.json
tsc

# Compile in watch mode
tsc --watch

# Run TypeScript directly with ts-node
npx ts-node file.ts

# Run in development with nodemon
npx nodemon --exec ts-node file.ts

# Run tests with Jest
npx jest

# Run with Node.js after compilation
node file.js

# Run in a web browser
# Include compiled .js files in HTML

# Type checking only (no output)
tsc --noEmit

# Build for production
npm run build
```

## Common Libraries

- **Web Frameworks**: React, Angular, Vue.js, Svelte
- **Backend Frameworks**: Express.js, NestJS, Fastify, Koa
- **Testing**: Jest, Mocha, Jasmine, Cypress
- **State Management**: Redux, MobX, Zustand
- **UI Libraries**: Material-UI, Chakra UI, Tailwind CSS
- **API Clients**: Axios, fetch
- **Validation**: Zod, Yup, io-ts, class-validator
- **GraphQL**: Apollo Client, URQL, graphql-request
- **Utility**: Lodash, date-fns, Ramda
- **Server-side Rendering**: Next.js, Remix, Gatsby
- **ORM**: Prisma, TypeORM, Sequelize
- **Developer Tools**: ESLint, Prettier, ts-node
- **Documentation**: TypeDoc, Storybook
- **Monorepo**: Nx, Turborepo, Lerna
