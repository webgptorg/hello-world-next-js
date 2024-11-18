# ✨ Hello World!

Welcome! In this repository, you'll find a simple example of how to write your first [Book](https://github.com/webgptorg/book) and run it using the [Promptbook Engine](https://github.com/webgptorg/promptbook) via the CLI.

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
