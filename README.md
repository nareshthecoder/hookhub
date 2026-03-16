# HookHub

HookHub is a modern web application built with [Next.js](https://nextjs.org), [TypeScript](https://www.typescriptlang.org/), and [Tailwind CSS](https://tailwindcss.com). It provides a centralized hub for managing and monitoring webhooks, enabling seamless event-driven integrations between services.

## Tech Stack

| Technology | Version | Purpose |
|---|---|---|
| [Next.js](https://nextjs.org) | 16.x | React framework with App Router |
| [React](https://react.dev) | 19.x | UI library |
| [TypeScript](https://www.typescriptlang.org/) | 5.x | Type-safe JavaScript |
| [Tailwind CSS](https://tailwindcss.com) | 4.x | Utility-first CSS framework |
| [ESLint](https://eslint.org/) | 9.x | Code linting |

## Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) v18.18 or later
- [npm](https://www.npmjs.com/) v9+, [yarn](https://yarnpkg.com/), [pnpm](https://pnpm.io/), or [bun](https://bun.sh/)

## Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/nareshthecoder/hookhub.git
cd hookhub
npm install
```

## Getting Started

Run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

The app supports hot-reloading — changes to source files are reflected immediately without restarting the server.

## Project Structure

```
hookhub/
├── app/                  # Next.js App Router pages and layouts
│   ├── layout.tsx        # Root layout (shared across all pages)
│   └── page.tsx          # Home page
├── public/               # Static assets (images, icons, etc.)
├── next.config.ts        # Next.js configuration
├── tailwind.config.ts    # Tailwind CSS configuration
├── tsconfig.json         # TypeScript configuration
├── eslint.config.mjs     # ESLint configuration
├── postcss.config.mjs    # PostCSS configuration
└── package.json          # Project dependencies and scripts
```

## Available Scripts

| Script | Description |
|---|---|
| `npm run dev` | Start the development server with hot-reloading |
| `npm run build` | Build the application for production |
| `npm run start` | Start the production server (requires `build` first) |
| `npm run lint` | Run ESLint to check for code issues |

## Configuration

### Next.js

The Next.js configuration lives in [`next.config.ts`](./next.config.ts). Refer to the [Next.js configuration docs](https://nextjs.org/docs/app/api-reference/next-config-js) for available options.

### TypeScript

TypeScript options are defined in [`tsconfig.json`](./tsconfig.json). The project uses strict mode for maximum type safety.

### Tailwind CSS

Tailwind configuration is in [`tailwind.config.ts`](./tailwind.config.ts). The project uses Tailwind v4 which supports CSS-first configuration.

## Deployment

### Deploy on Vercel (recommended)

The easiest way to deploy HookHub is with the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme):

1. Push your code to a GitHub repository.
2. Import the project into Vercel.
3. Vercel will auto-detect Next.js and configure the build settings.
4. Your app will be live at a `*.vercel.app` URL.

### Self-hosted Deployment

Build and start the production server manually:

```bash
npm run build
npm run start
```

The production server listens on port `3000` by default. Use the `PORT` environment variable to override:

```bash
PORT=8080 npm run start
```

For detailed deployment options, see the [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying).

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Make your changes and commit: `git commit -m "feat: add your feature"`
4. Push to your fork: `git push origin feature/your-feature-name`
5. Open a pull request against the `main` branch.

Please ensure your code passes linting before submitting:

```bash
npm run lint
```

## Learn More

- [Next.js Documentation](https://nextjs.org/docs) — Next.js features and API reference
- [Learn Next.js](https://nextjs.org/learn) — interactive tutorial
- [Next.js GitHub Repository](https://github.com/vercel/next.js)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html)

## License

This project is private and not licensed for public use.
