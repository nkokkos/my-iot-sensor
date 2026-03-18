# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

## Installation

```bash
yarn
```

## Local Development

```bash
yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

## Build

```bash
yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

## Deployment

Using SSH:

```bash
USE_SSH=true yarn deploy
```

Not using SSH:

```bash
GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.

## Running it from local dev box
npm run serve -- --port 3001 --host 0.0.0.0

## Force clean deployment
# 1. Clean any old build files
npm run clear

# 2. Run the deploy command with your GitHub info
# Replace <YOUR_TOKEN> with your Personal Access Token
GIT_USER=github_user GITHUB_TOKEN=<YOUR_TOKEN> npm run deploy
