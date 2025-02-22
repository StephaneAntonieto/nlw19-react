# NLW19 - Reactjs - Nextjs 

This project was developed during NLW19 by Rocketseat. It is an application that allows event participation registration and referral of other people to the same event. Referrals are tracked and displayed in a ranking system.

## Features

- Event participation registration
- Generation of unique invitation links for each participant
- Tracking of accesses and registrations through invitation links
- Display of ranking with the best referrals

## Technologies Used

- **Frontend:**
  - React
  - Next.js
  - Tailwind CSS
  - TypeScript

- **Backend:**
  - Fastify
  - PostgreSQL
  - Redis
  - Drizzle ORM
  - TypeScript

## Project Structure

### Frontend

The frontend of the application is located in the `src/app` folder. It is responsible for rendering the pages and components of the application, as well as making requests to the backend.

### Backend

The backend of the application is located in the `api/src` folder. It is responsible for managing routes, connecting to the database and Redis, and processing business logic.

### ScreenShots

| ![Imagem 1](/screenshot/RegisterScreen.svg) | ![Imagem 2](/screenshot/RankingScreen.svg) |
|--------------------------|--------------------------|

## How to Run the Project

### Prerequisites

- Node.js
- Docker

### Steps to Run

1. Clone the repository:
```sh
    git clone https://github.com/stephaneantonieto/nlw19.git
    cd nlw19
```
2. Install frontend dependencies:
```sh
    cd web
    npm install
```
3. Install backend dependencies:
```sh
    cd web/api
    npm install
```
4. Configure environment variables:
   - Create a `.env` file in the `api` folder with the following variables:
```sh
    PORT=3333
    DATABASE_URL=your_postgresql_url
    REDIS_URL=your_redis_url
    API_URL=http://localhost:3333
    WEB_URL=http://localhost:3000
```
5. Run backend services:
```sh
    cd web/api
    docker-compose up
    npm run dev
```
6. Run frontend:
```sh
    cd web
    npm run dev
```
7. Access the application at `http://localhost:3000`
