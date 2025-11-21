# QUICKSTART

Quick guide to get the project up and running locally.

## Prerequisites

- **Node.js 12.x** - This project uses node-sass which requires Node 12
- **npm** - Comes with Node.js

## Setup

### 1. Install Node 12

This project uses Node.js version 12.22.12. We recommend using [nvm](https://github.com/nvm-sh/nvm) to manage Node versions.

If you have nvm installed, simply run:

```bash
nvm use
```

This will automatically use the Node version specified in `.nvmrc`.

If you don't have Node 12 installed yet, install it with:

```bash
nvm install 12
nvm use 12
```

### 2. Install Dependencies

```bash
npm install
```

This will install all dependencies based on the lockfile (`package-lock.json`), ensuring reproducible builds.

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

If you encounter errors related to node-sass or native modules, ensure you're using Node 12:

```bash
node --version
# Should output: v12.22.12
```

If it shows a different version, run `nvm use 12` again.

### Clean Install

If you're experiencing issues with dependencies:

```bash
rm -rf node_modules package-lock.json
npm install
```

## Tech Stack

- [Gridsome](https://gridsome.org/) | [Vue.js](https://vuejs.org/)
- [TailwindCSS](https://tailwindcss.com/) | SCSS
- [Forestry CMS](https://forestry.io/)
- [Netlify](https://www.netlify.com/)
