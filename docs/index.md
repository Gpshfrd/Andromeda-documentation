# Welcome to Andromeda online-store!

## Overview

Andromeda is a platform for managing an online store, featuring a Django backend and a React frontend. The project supports product management, orders, cart, users, and delivery.

## Quick Start

**Backend**

Install dependencies:
```
pip install -r requirements.txt
```

Apply migrations:
```
python manage.py migrate
```

Start the server:
```
python manage.py runserver
```

**Frontend**

Install dependencies:
```
npm install
```

Start the dev server:

```
npm run dev
```

##  Project Structure

- andromeda/ — Django backend
    - api/ — API endpoints, serializers, views
    - carts/, deliveries/, orders/, products/, users/ — business logic and models
    - templates/, static/ — templates and static files
- frontend/ — React application
    - src/ — source code (widgets, features, entities, pages, shared)
    - public/ — static files

## Backend Overview

- Uses Django 4+
- Main apps: carts, deliveries, orders, products, users
- REST API implemented in andromeda/api/
- Authentication via standard Django mechanisms

## Frontend Overview

- Uses React + Vite + TypeScript
- Architecture split into widgets, features, entities, pages, shared
- Styling with PostCSS
- Interacts with backend via REST API

## API Reference

- Base URL: /api/
- Example endpoints:
    - /api/products/ — product list
    - /api/orders/ — create and view orders
    - /api/carts/ — cart operations
- Authentication: JWT or sessions (specify as per your project)

[link to swagger] (will be added later)

## User Guide

## Admin Guide

## Testing

How to run backend tests:

```
python manage.py test
```

How to run frontend tests:

```
npm run test (if implemented)
```