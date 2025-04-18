# Node.js Installation Guide

## Required Software

- **Node.js**: JavaScript runtime environment
- **npm**: Node Package Manager (included with Node.js)
- **nvm**: Node Version Manager (recommended for managing multiple Node.js versions)
- **VS Code**: Popular editor with JavaScript/Node.js support
- **Git**: For version control and package installation

## File Extensions

- `.js` - JavaScript source files
- `.mjs` - ES modules JavaScript files
- `.cjs` - CommonJS modules files
- `.jsx` - JavaScript with JSX syntax
- `.ts` - TypeScript files
- `.json` - JSON configuration files
- `.node` - Compiled native addon modules
- `package.json` - Project configuration and dependencies
- `package-lock.json` - Dependency lock file
- `.nvmrc` - Node version file for nvm
- `.npmignore` - Files to exclude from npm packages
- `.npmrc` - npm configuration file

## Package Management

```bash
# Install Node.js using NVM (recommended)
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
nvm install node  # Latest version
nvm install 16    # Specific version (e.g., 16.x)

# Install a package globally
npm install -g package-name

# Initialize a new project
npm init

# Install project dependencies
npm install

# Install and save a dependency
npm install --save package-name

# Install and save a dev dependency
npm install --save-dev package-name

# Update packages
npm update

# Remove a package
npm uninstall package-name

# Using Yarn (alternative package manager)
yarn add package-name
yarn remove package-name
yarn upgrade
```

## Running Node.js Programs

```bash
# Run a JavaScript file
node app.js

# Run with ES modules
node --experimental-modules app.mjs

# Run with environment variables
NODE_ENV=production node app.js

# Run with debugging
node --inspect app.js

# Run with automatic restart (using nodemon)
nodemon app.js

# Run npm scripts (defined in package.json)
npm run start
npm run dev
npm run test

# Run in REPL (interactive) mode
node
```

## Common Libraries

- **Web Frameworks**: Express, Koa, Fastify, NestJS
- **API**: REST, GraphQL (Apollo, Express-GraphQL)
- **Database**: Mongoose (MongoDB), Sequelize (SQL), Prisma
- **Testing**: Jest, Mocha, Chai
- **Authentication**: Passport, JWT
- **Utility**: Lodash, Ramda
- **Async Flow**: Async.js, Promises, Observables (RxJS)
- **Process Management**: PM2, Forever
- **Templates**: EJS, Pug, Handlebars
- **CLI Tools**: Commander, Yargs
- **HTTP Clients**: Axios, node-fetch, got
