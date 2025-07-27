# Password Manager Application

## Overview

This is a Password Manager Application.

## Getting Started

### Git Clone

Please git clone This repository
This repository use submodule So, Please git clone under the repositories
next-password-manager-app(<https://github.com/lee266/next-password-manager-app.git>)
next-password-manager-api(<https://github.com/lee266/next-password-manager-api.git>)

```sh
git clone https://github.com/lee266/next-password-manager-monorepo.git
cd next-password-manager-monorepo

# Clone frontend
cd app
git clone https://github.com/lee266/next-password-manager-app.git

# Clone backend
cd ../api
git clone https://github.com/lee266/next-password-manager-api.git
```

### Active Project

Please copy .env　and write .env file

```sh
cp .env.example .env
cd api
cp .env.example .env
```

To launch the project using Docker, run the following command:

```sh
docker compose up -d --build
# Then, apply database migrations (only required on first run)
docker compose exec -T django python manage.py migrate
```

This command initializes and starts the containers necessary for both the frontend and backend components.

## Environments

- Frontend
  - Next.js
  - Material UI
  - Yarn
- Backend
  - Python
  - Django
- Code Hosting
  - GitHub
- Builders
  - Vercel
  - Render

## Architecture

- Production infrastructure diagram: ./doc/infrastructure/infra.pu
- Development infrastructure diagram: ./doc/infrastructure/infra-dev.pu

## hints

Naming Conventions
PascalCase: CurrentUserItem
CamelCase: currentUserItem
SnakeCase: current_user_item
KebabCase: current-user-item

- directory
-- first layer
  - lowerCase
-- other layer
  - PascalCase
- component file
PascalCase
- other
KebabCase
