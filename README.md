# Next.js + Convex Starter Template

A modern, production-ready template combining Next.js 15+ and Convex backend for building real-time web applications.

## Features

- **Next.js 15+**: Latest version with App Router for optimal performance
- **Convex Backend**: Real-time database and backend as a service
- **TypeScript**: End-to-end type safety
- **Tailwind CSS**: Utility-first CSS framework
- **pnpm**: Fast, disk space efficient package manager
- **Modern React**: Leveraging React 19 features
- **Geist Font**: Beautiful typography from Vercel

## Getting Started

### Prerequisites

- Node.js 18.17.0 or later
- pnpm package manager
- Convex account (free tier available)

### Installation

1. Clone the repository:

```bash
git clone https://github.com/sorryshady/next_convex_starter.git
cd next_convex_starter
```

2. Install dependencies:

```bash
pnpm install
```

3. Set up Convex:

```bash
npx convex dev
```

This will prompt you to log in to your Convex account and create a new deployment.

4. Start the development server:

```bash
pnpm dev
```

5. Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Project Structure

```
/
├── app/                    # Next.js app directory
│   ├── layout.tsx          # Root layout
│   ├── page.tsx            # Home page
│   └── globals.css         # Global styles
├── convex/                 # Convex backend
│   ├── _generated/         # Generated Convex files (do not edit)
│   ├── schema.ts           # Database schema definition
│   └── ...                 # Convex functions
├── lib/                    # Shared utilities
├── public/                 # Static assets
├── components.json         # UI component configuration
└── package.json            # Project dependencies
```

## Convex Backend

The Convex backend provides:

- Real-time data synchronization
- Automatic database migrations
- TypeScript-first developer experience
- Serverless functions for queries and mutations

To learn more about using Convex with Next.js, check out the [Convex documentation](https://docs.convex.dev/nextjs).

## Development Workflow

1. Define your data schema in `convex/schema.ts`
2. Create your backend functions in `convex/*.ts` files
3. Use the generated API client in your React components

## Deployment

### Deploy on Vercel

The easiest way to deploy your Next.js app is to use [Vercel](https://vercel.com/new).

1. Push your code to a Git repository
2. Import the project to Vercel
3. Add your Convex deployment URL as an environment variable

### Deploy Convex Backend

Your Convex backend will automatically deploy when you push your code if you set up Convex's GitHub integration.

## Learn More

- [Next.js Documentation](https://nextjs.org/docs)
- [Convex Documentation](https://docs.convex.dev)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)

## License

MIT
