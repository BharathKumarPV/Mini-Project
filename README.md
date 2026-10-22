# KisanConnect

India's Agriculture Market, Connected.

This repository contains the source code for KisanConnect, a full-stack app for mandi price tracking, market comparison, and a farmer-to-buyer marketplace.

## Stack
- Frontend: React, Vite, TypeScript, Tailwind CSS
- Backend: Node.js, Express, TypeScript
- Database: SQLite with Prisma ORM
- Price data: data.gov.in AGMARKNET API

## Requirements
- Node.js 18+
- npm 9+

## Setup

1. Install dependencies from the repository root:

   ```bash
   npm run install:all
   ```

2. Configure the backend environment:

   ```bash
   cp backend/.env.example backend/.env
   ```

   Set a strong `JWT_SECRET` and optionally set `DATA_GOV_API_KEY` for live price synchronization.

3. Create and seed the local database:

   ```bash
   npm run db:setup
   ```

4. Start both servers:

   ```bash
   npm run dev
   ```

Frontend: http://localhost:5173  
Backend health check: http://localhost:3000/health

See the application source and package scripts for additional details. Do not commit `.env` files or real API keys.
