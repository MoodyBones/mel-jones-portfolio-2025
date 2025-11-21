# QUICKSTART

Quick guide to get the project up and running locally.

## Prerequisites

- **Node.js 16.x or higher** - This project uses dart-sass which supports modern Node versions
- **npm** - Comes with Node.js

## Setup

### 1. Install Node

This project recommends Node.js version 16.20.2. We recommend using [nvm](https://github.com/nvm-sh/nvm) to manage Node versions.

If you have nvm installed, simply run:

```bash
nvm use
```

This will automatically use the Node version specified in `.nvmrc`.

If you don't have the recommended Node version installed yet, install it with:

```bash
nvm install
nvm use
```

### 2. Install Dependencies

```bash
npm ci
```

This will install all dependencies using the exact versions specified in the lockfile (`package-lock.json`), ensuring reproducible builds.

### 3. Run Development Server

```bash
npm run develop
```

The site will be available at `http://localhost:8080` (or the port Gridsome assigns).

## Available Scripts

- `npm run develop` - Start development server
- `npm run build` - Build for production
- `npm run explore` - Explore GraphQL data layer

## Troubleshooting

### Node Version Issues

If you encounter errors, ensure you're using a compatible Node version (16.x or higher):

```bash
node --version
# Should output: v16.20.2 or higher
```

If it shows a different version, run `nvm use` again.

### Clean Install

If you're experiencing issues with dependencies, try a clean install using the lockfile:

```bash
rm -rf node_modules
npm ci
```

Note: `npm ci` (clean install) uses the exact versions from package-lock.json, ensuring reproducible builds.

## Tech Stack

- [Gridsome](https://gridsome.org/) | [Vue.js](https://vuejs.org/)
- [TailwindCSS](https://tailwindcss.com/) | SCSS
- [Forestry CMS](https://forestry.io/)
- [Netlify](https://www.netlify.com/)
