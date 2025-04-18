# JavaScript Installation Guide

## Required Software

- **Node.js**: Download and install from [nodejs.org](https://nodejs.org/) (LTS version recommended)
- **npm**: Package manager (included with Node.js installation)
- **nvm** (optional): For managing multiple Node.js versions, install from [github.com/nvm-sh/nvm](https://github.com/nvm-sh/nvm)

## File Extensions

- `.js` - JavaScript source files
- `.jsx` - React JavaScript files
- `.mjs` - ES modules
- `.cjs` - CommonJS modules
- `.json` - JSON data files
- `.ts` - TypeScript files (requires TypeScript compiler)
- `.html` - HTML files (when used with embedded JavaScript)

## Package Management

```bash
# Initialize a new project
npm init

# Install packages
npm install package-name

# Install dev dependencies
npm install --save-dev package-name

# Save dependencies in package.json
# Install from package.json
npm install
```

## Running JavaScript Programs

```bash
# Run with Node.js
node script.js

# Run with npm script (defined in package.json)
npm run script-name

# Interactive REPL
node
```

## Common Libraries

- **Frontend**: React, Vue.js, Angular, Svelte
- **Backend**: Express, Nest.js, Fastify, Koa
- **Testing**: Jest, Mocha, Chai
- **Utilities**: Lodash, Moment.js, Axios
