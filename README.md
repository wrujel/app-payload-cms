<div align="center">
  <h1>CMS using Payload and Mongodb</h1>
</div>

<div align="center">
  <a href="/README.md">
    <img 
      src="https://img.shields.io/badge/Status-Complete-success.svg" 
      alt="Status" 
    />
  </a>
  <a href="/package.json">
    <img 
      src="https://img.shields.io/badge/Version-1.0.0-blue.svg" 
      alt="Version" 
    />
  </a>
  <a href="/LICENSE">
    <img 
      src="https://img.shields.io/badge/License-MIT-green.svg" 
      alt="License" 
    />
  </a>
  <a href="https://www.typescriptlang.org/">
    <img 
      src="https://img.shields.io/badge/TypeScript-4.3.5-blue?style=flat&logo=typescript" 
      alt="TypeScript 4.3.5" 
    />
  </a>
  <a href="https://www.mongodb.com/">
    <img 
      src="https://img.shields.io/badge/MongoDB-4.4.6-blue?style=flat&logo=mongodb" 
      alt="MongoDB 4.4.6" 
    />
  </a>
  <a href="https://expressjs.com/">
    <img 
      src="https://img.shields.io/badge/Express-4.17.1-blue?style=flat&logo=express" 
      alt="Express 4.17.1" 
    />
  </a>
  <a href="https://payloadcms.com/">
    <img 
      src="https://img.shields.io/badge/Payload-3.0.0-blue?style=flat&logo=payload" 
      alt="Payload 3.0.0" 
    />
  </a>
  <a href="https://www.docker.com/">
    <img 
      src="https://img.shields.io/badge/Docker-20.10.7-blue?style=flat&logo=docker" 
      alt="Docker 20.10.7" 
    />
  </a>
</div>
<br />

This is a project to create a CMS to manage users and products for a store. It is built using a blank Payload CMS template, express, typescript and mongodb. 

# Table of Contents
- [Table of Contents](#table-of-contents)
- [Tech Stack](#tech-stack)
- [Payload Blank Template](#payload-blank-template)
  - [Development](#development)
    - [Docker](#docker)
  - [Production](#production)
    - [Deployment](#deployment)
  - [Questions](#questions)

# Tech Stack
- Nodejs
- Express
- MongoDB
- Typescript
- Payload CMS
- Docker

# Payload Blank Template

A blank template for [Payload](https://github.com/payloadcms/payload) to help you get up and running quickly. This repo may have been created by running `npx create-payload-app@latest` and selecting the "blank" template or by cloning this template on [Payload Cloud](https://payloadcms.com/new/clone/blank).

See the official [Examples Directory](https://github.com/payloadcms/payload/tree/main/examples) for details on how to use Payload in a variety of different ways.

## Development

To spin up the project locally, follow these steps:

1. First clone the repo
1. Then `cd YOUR_PROJECT_REPO && cp .env.example .env`
1. Next `yarn && yarn dev` (or `docker-compose up`, see [Docker](#docker))
1. Now `open http://localhost:3000/admin` to access the admin panel
1. Create your first admin user using the form on the page

That's it! Changes made in `./src` will be reflected in your app.

### Docker

Alternatively, you can use [Docker](https://www.docker.com) to spin up this project locally. To do so, follow these steps:

1. Follow [steps 1 and 2 from above](#development), the docker-compose file will automatically use the `.env` file in your project root
1. Next run `docker-compose up`
1. Follow [steps 4 and 5 from above](#development) to login and create your first admin user

That's it! The Docker instance will help you get up and running quickly while also standardizing the development environment across your teams.

## Production

To run Payload in production, you need to build and serve the Admin panel. To do so, follow these steps:

1. First invoke the `payload build` script by running `yarn build` or `npm run build` in your project root. This creates a `./build` directory with a production-ready admin bundle.
1. Then run `yarn serve` or `npm run serve` to run Node in production and serve Payload from the `./build` directory.

### Deployment

The easiest way to deploy your project is to use [Payload Cloud](https://payloadcms.com/new/import), a one-click hosting solution to deploy production-ready instances of your Payload apps directly from your GitHub repo. You can also deploy your app manually, check out the [deployment documentation](https://payloadcms.com/docs/production/deployment) for full details.

## Questions

If you have any issues or questions, reach out to us on [Discord](https://discord.com/invite/payload) or start a [GitHub discussion](https://github.com/payloadcms/payload/discussions).
