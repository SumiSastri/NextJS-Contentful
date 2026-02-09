
# Scaffolding

1. Update packages

```bash
# Remove existing node modules and lock file update node version
rm -rf node_modules
rm -rf build
rm -rf public
rm package-lock.json
nvm install 24.13.0   
npm install
```

Ensure you have the right version of node

- [Node and nvm install guide from freecodecamp for ongoing package management](https://www.freecodecamp.org/news/node-version-manager-nvm-install-guide/)

- Using [nvm](https://github.com/nvm-sh/nvm#installing-and-updating)

- Keeping the [.nvmrc file](https://kl1p.com/what-you-need-to-know-about-nvmrc-tips-and-tricks-with-step-by-step-code-examples/) up to date in the root of the repo

2.Check deps

- Latest version of [nextJS](https://www.npmjs.com/package/next)
- [Next.js](https://nextjs.org/)
- Note Next does not have a `src` folder by default now - all code is in the root or `app` folder
- [Next.js Documentation](https://nextjs.org/docs) 
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

```json
# Ensure the following package versions are in your `package.json` file
    "autoprefixer": "10.4.16",
    "eslint": "9.39.2",
    "eslint-config-next": "16.1.6",
    "next": "16.1.5",
    "postcss": "8.4.31",
    "react": "18.2.0",
    "react-dom": "18.2.0",
    "tailwindcss": "3.3.5"
```

3.Install with npm `npm install` and check dev server runs `npm run dev` check local host
 `http://localhost:3000/events/nov-2023` are in nested folders in the app folder

4.JSON Server

[JSON Server](https://www.npmjs.com/package/json-server) is a simple way to create a REST API with fake data. It is useful for prototyping and mocking during development.

Install globally `npm install json-server -g`
Keep 2 terminals open - backend and frontend

`json-server --watch --port 4000 ./_db/db.json`
Open terminal 1 [http://localhost:4000/tickets](http://localhost:4000/tickets) check backend data renders
`npm run dev`
Open terminal 2 [http://localhost:3000/tickets}](http://localhost:3000/tickets) check backend data renders in frontend

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

4.Sample dot-env file

`npx cross-env CONTENTFUL_ACCESS_TOKEN="paste your contentful access token here"  

- this sample.env file is for local development - ensure you have the correct values from your Contentful account and API keys

```env
CONTENTFUL_ACCESS_TOKEN="paste your contentful access token here"
CONTENTFUL_ENVIRONMENT=paste your contentful environment here - master, dev etc.
CONTENTFUL_MANAGEMENT_TOKEN=paste your CFPAT here
CONTENTFUL_PREVIEW_ACCESS_TOKEN="paste your contentful preview access token here"
CONTENTFUL_PREVIEW_SECRET="paste your contentful preview secret here"
CONTENTFUL_REVALIDATE_SECRET="paste your contentful revalidate secret here"
CONTENTFUL_SPACE_ID=paste your contentful space id here
NEXT_ENV="paste your environment here - dev, staging, prod etc."
API_URL="paste your api url here"
DB_URL="paste your db url here"
INFRA_URL="paste your infrastructure url here"
```
