# Tattoo One Love — Strapi CMS

<div align="center">

<img alt="Strapi" src="https://img.shields.io/badge/Strapi-v3.1.5-2E7EEA?logo=strapi&logoColor=white" />
<img alt="Node.js" src="https://img.shields.io/badge/Node.js-12.x-339933?logo=node.js&logoColor=white" />
<img alt="SQLite" src="https://img.shields.io/badge/SQLite-3-003B57?logo=sqlite&logoColor=white" />

</div>

## Overview

Headless CMS for the Tattoo One Love website built with Strapi v3. It provides an admin panel and REST API to manage site content such as mission, works portfolio, newsletter emails, and legal pages.

## Key Features

- Structured content models: `our-mission`, `our-works`, `important-message`, `newsletter-emails`, and legal policies
- Media library with file uploads and asset management
- Authentication and role-based access via Users & Permissions plugin

## Tech Stack

Node.js 12, Strapi 3.1.5, SQLite 3 (Bookshelf/Knex)

## Architecture

Strapi v3 application exposing REST endpoints, using Bookshelf ORM and SQLite (dev). Core plugins include Content Manager, Content Type Builder, Upload, Email, and Users & Permissions. Configuration lives under `config/` with environment-driven settings.

## Performance & Accessibility

Static asset handling via the Upload plugin; admin UI built by Strapi. No custom caching layer is configured.

## Prerequisites

- Node.js: `12.x LTS`

## Installation

```bash
git clone https://github.com/maxgalchenko/tattoo-one-love--strapi.git
cd tattoo-one-love--strapi
npm install
```

## Environment Variables

```env
HOST=0.0.0.0
PORT=1337
ADMIN_JWT_SECRET=replace-with-strong-secret
DATABASE_FILENAME=.tmp/data.db
```

## Quick Start

```bash
npm run develop
# Production
npm run build
npm start
```

Open http://localhost:1337/admin

## Available Scripts

- `npm run develop` – Start Strapi in watch mode with live-reload
- `npm run build` – Build the Strapi admin panel
- `npm start` – Run Strapi in production mode
- `npm run strapi` – Access the Strapi CLI

---

<div align="center">

Built with ❤️ by [Maksym Galchenko](https://github.com/maxgalchenko)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/galchenko-max/)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-green?style=for-the-badge&logo=web)](https://portfolio-green-six-29.vercel.app/)
[![Email](https://img.shields.io/badge/Email-Contact-red?style=for-the-badge&logo=gmail)](mailto:galchenko.maksym@gmail.com)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

</div>
