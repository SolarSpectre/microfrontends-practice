# Microfrontend Practice with `create-mf-app`

This repository contains a project for exploring and practicing microfrontend architecture using the `create-mf-app` tool. The goal is to build modular, independent frontend applications that can be integrated seamlessly into a single application.

## About `create-mf-app`

`create-mf-app` is a CLI tool for setting up a microfrontend environment quickly. It scaffolds multiple applications with shared dependencies, enabling efficient development and deployment of microfrontend applications.

## Features

- Modular structure for each frontend application
- Shared dependencies to reduce bundle size
- Independent deployment of each micro-app
- Configured with Webpack Module Federation for smooth integration

## Getting Started

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/) (>=14.x recommended)
- [pnpm](https://pnpm.io/) for package management

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/SolarSpectre/microfrontends-practice.git
   cd microfrontends-practice
   ```

2. Install dependencies for each microfrontend application:

```bash
pnpm install
```

### Running the applications

To start the microfrontend apps in development mode:

```bash
pnpm start
```

### Project Structure

    /host - SolidJS app that consumes the microfrontend from the remote app.
    /remote - The microfrontend application.
    /react-host - The React application that consumes the microfrontend from the remote app.

### Technologies Used

    React and SolidJS for UI cross-platform components
    Webpack Module Federation for sharing code across microfrontends
    create-mf-app CLI for scaffolding the project
