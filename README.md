# ManageStack Frontend

**ManageStack** is the Next.js frontend for a full‑stack Project Management App, connecting to a Go backend and AWS services. It provides a responsive UI for managing projects, tasks, and collaboration in real time.

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Environment Variables](#environment-variables)
  - [Running Locally](#running-locally)
- [Available Scripts](#available-scripts)
- [Folder Structure](#folder-structure)
- [Deployment](#deployment)
- [Learn More](#learn-more)

## Features

- ✅ User authentication (JWT/Cognito)
- ✅ Project and task CRUD operations
- ✅ Kanban board drag‑and‑drop (react‑beautiful‑dnd)
- ✅ Data visualizations with Recharts
- 🌓 Light/Dark mode toggle
- 📋 Form validation with React Hook Form & Zod

## Tech Stack

- **Next.js** 15 (App Router)
- **React** 19 & **TypeScript**
- **Tailwind CSS** (utility‑first styling)
- **MUI** (Material UI components)
- **Redux Toolkit** (state management)
- **Recharts** (charts & graphs)
- **Syncfusion Gantt** (project timeline)
- **AWS Amplify** / **Vercel** for deployment

## Prerequisites

- Node.js >= 18
- npm or yarn
- (Optional) AWS CLI & Amplify CLI if deploying on AWS

## Getting Started

### Installation

```bash
git clone https://github.com/your-username/ManageStack.git
cd ManageStack
npm install
# or
yarn install
```

### Environment Variables

Create a `.env.local` at the project root with:

```env
NEXT_PUBLIC_API_URL=http://localhost:8000/api
NEXT_PUBLIC_COGNITO_USER_POOL_ID=us-east-1_xxxxx
NEXT_PUBLIC_COGNITO_CLIENT_ID=xxxxxxxxxxxx
```

### Running Locally

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Available Scripts

- `npm run dev`: Start development server
- `npm run build`: Build for production
- `npm run start`: Run production server
- `npm run lint`: Run ESLint

## Folder Structure

```
src/
├── app/          # Next.js App Router (layouts & pages)
├── components/   # Reusable UI components
├── context/      # React context providers
├── hooks/        # Custom React hooks
├── styles/       # Global CSS & Tailwind imports
├── utils/        # Helpers & utilities
└── public/       # Static assets
```

## Deployment

### Vercel

1. Push to GitHub.
2. Import into Vercel.
3. Configure environment variables in Vercel Dashboard.

### AWS Amplify

1. Initialize: `amplify init`
2. Add hosting: `amplify add hosting`
3. Publish: `amplify publish`

## Learn More

- **Next.js Docs**: [https://nextjs.org/docs](https://nextjs.org/docs)
- **Tailwind CSS Docs**: [https://tailwindcss.com/docs](https://tailwindcss.com/docs)
- **AWS Amplify Docs**: [https://docs.amplify.aws/](https://docs.amplify.aws/)

