# How to Install and Use TypeScript with tsc Watch

###### TypeScript is a statically typed superset of JavaScript that helps you write more maintainable and error-free code. In this guide, we'll walk you through the process of installing TypeScript and using the TypeScript Compiler (tsc) with the --watch flag for automatic code compilation.

## Prerequisites

Before you begin, make sure you have the following installed on your system:
Node.js and npm (Node Package Manager)

## Installation

### Install TypeScript globally

(if you prefer a local installation, skip this step):

```bash
npm install -g typescript
```

This command installs TypeScript globally, making it available system-wide.

### Initialize your project by creating a package.json file:

```bash
npm init -y
```

This command generates a basic package.json file for your project.

### Install TypeScript locally (if you didn't install it globally):

```bash
npm install typescript --save-dev
```

This command installs TypeScript as a development dependency for your project.

## Usage

#### Create Typescript Files

Create TypeScript files with the .ts extension in your project directory. For example, app.ts

#### Create a tsconfig.json file

Create a tsconfig.json file in your project directory to configure TypeScript options:

```bash
touch tsconfig.json
```

Edit tsconfig.json and add the following minimal configuration:

```bash
{
  "compilerOptions": {
    "target": "ES6",
    "outDir": "dist"
  },
  "include": ["**/*.ts"]
}
```

This configuration specifies that TypeScript should target ECMAScript 6 and compile TypeScript files in the current directory and its subdirectories, placing the compiled JavaScript files in a dist directory.

You can further customize the tsconfig.json file according to your project requirements.

#### Compile TypeScript Code

    To compile your TypeScript code, open your terminal and run:
