# ✨ Hello World!

Welcome! In this repository, you'll find a simple example of how to write your first [Book](https://github.com/webgptorg/book) and run it using the [Promptbook Engine](https://github.com/webgptorg/promptbook) via the CLI.


> TODO: !!!!!! Merge Book and Next Getting Started

## Getting Started

Follow these steps to get up and running:

### 1. Clone the Repository
First, clone this repository to your local machine.

### 2. Install Promptbook
Navigate to the root of the project and run the following command to install Promptbook:

```bash
npm i ptbk
```

**Note:** Currently, installation is supported only via NPM. We are actively working on adding support for other package managers and installer files such as `.msi`, `.rpm`, and `.deb`.

### 3. Configure Environment Variables
Create a `.env` file in the root of the project to configure the necessary API keys for the model providers you plan to use:

```conf
# You only need to configure one provider:

# OpenAI
OPENAI_API_KEY=sk-proj-...

# Anthropic Claude
ANTHROPIC_CLAUDE_API_KEY=sk-ant-api03-...

# Azure OpenAI
AZUREOPENAI_API_KEY=...
AZUREOPENAI_RESOURCE_NAME=...
AZUREOPENAI_DEPLOYMENT_NAME=...
```

### 4. Run the Example
From the root of the repository, execute the following command to run the example:

```bash
npx ptbk books/hello.book.md
```

### Expected Output
If everything is set up correctly, you should see the following output:

```bash
$ npx ptbk books/hello.book.md
√ yourName ... The World

--- Result: ---
greeting: Hello World!
```

🚀✨ **Congratulations!** You've successfully created **your first book** with Promptbook! Now you can [continue with the examples](/books/) or [the book language blueprint](https://github.com/webgptorg/book) to dive deeper into the book language, [integrate books into your app]() or [create instant miniapps](#!!!!!!) without classical programming.


This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
