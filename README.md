# Repo access

Pre-requisistes:

- Node v.20 or higher and nvm [install guide from freecodecamp for ongoing package management](https://www.freecodecamp.org/news/node-version-manager-nvm-install-guide/)
- Contenteful account with access to the space_ID and API keys
- NextJS v.16 or higher installed on your local machine 
- JSON Server installed globally `npm install json-server -g` for backend prototyping and mocking during development
- GitHub account with access to the repo and permissions to clone and push changes

# Getting Started

1. Clone the repo to your local machine using GitHub Desktop or command line `git clone <repo-url>`
2. Navigate to the project directory `cd nextjs-contentful`
3. Follow the scaffolding steps below to set up the project and run the development server
4. Make changes to the codebase and push to GitHub to see changes reflected in the deployed application

Scripts to run:

- `npm run dev` - runs the development server at `http://localhost:3000`
- `json-server --watch --port 4000 ./_db/db.json` - runs the JSON Server backend at `http://localhost:4000`
- `npm run build` - builds the application for production
- `npm start` - starts the production server after building

