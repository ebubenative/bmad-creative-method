# Installing the BMAD Creative Method

Welcome to the BMAD Creative Method! This guide will walk you through the simple process of installing the framework into your project.

## Quick Install

For the best experience, we recommend using the interactive installer. Open your terminal at the root of your project folder and run the following command:

```bash
git clone https://github.com/ebubenative/bmad-creative-method.git
cd bmad-creative-method
npm install
npm run install:bmad
```

This will launch an interactive setup process that will guide you through configuring the BMAD Creative Method for your specific project needs.

## Manual Installation

If you prefer to install the method manually, follow these steps:

1.  **Copy the `bmad-core` directory:** Copy the `bmad-core` directory from this repository into the root of your project folder.
2.  **Copy the `common` directory:** Copy the `common` directory into the root of your project folder.
3.  **Create a `.bmad` directory:** In the root of your project, create a new directory called `.bmad`.
4.  **Configure your project:** Inside the `.bmad` directory, create a `config.yaml` file. You can start by copying the `bmad-core/core-config.yaml` and then customizing it for your project.

## Getting Started

Once the installation is complete, you can start your first project by running the following command in your terminal:

```bash
bmad-agent exec maestro kickoff
```

The Maestro agent will then guide you through the rest of the setup process.

## For IDE Integration

The BMAD Creative Method is designed to work with a variety of Agentic IDEs. Please refer to your specific IDE's documentation for instructions on how to integrate custom agent frameworks. The key things you will need to provide are:

-   The path to the `bmad-core/agents` directory.
-   The command prefix you would like to use (e.g., `@` or `/`).

Welcome to a new era of creative workflow. We can't wait to see what you create!
