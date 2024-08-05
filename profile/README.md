
# Welcome to Voidara 👋

Welcome to the GitHub organization for Voidara. Here, you'll find a variety of tools and projects developed for the [Voidara Minecraft Server](https://voidara.net).

For questions or support, please visit our [Discord](https://discord.voidara.net)!

## Table of Contents

- 💻 [Our Technology](#-our-technology)
- 🦅 [Branching Strategy](#-branching-strategy)
- 📖 [Style Guide](#-style-guide)
- 💼 [Hiring](#-hiring)

## 💻 Our Technology

Our core server software is built using [Minestom](https://minestom.net/). We use PostgreSQL for structured data and MongoDB for unstructured data. Each game server operates independently and can be redeployed as needed, with all player data stored in the database. For deployment, we utilize Docker with a custom cloud system that adjusts the deployment of Docker containers based on player count.

## 🦅 Branching Strategy

At Voidara, we adhere to the `stable <- dev` branching strategy. This means the `stable` branch should always be deployable. Code is initially pushed to the `dev` or a `feature/<feature_name/id>` branch, which is later merged into `dev`. Once the `dev` branch is ready for release, it is merged into the `stable` branch via a pull request. This process ensures stability and provides a clear overview of changes.

Commit messages should be descriptive, ideally phrased to fit "When applied this commit will ...". For example:

Bad commit message:
```
+ DatabaseModule
```
Good commit message:
```
Add the DatabaseModule
```

## 📖 Style Guide

Readability and consistency are paramount at Voidara. Our style guide includes several principles derived from the [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html):

- **Source File Basics**
  - File encoding should be UTF-8.

- **Formatting**
  - Use two spaces for indentation, not tabs.
  - The column limit for code lines is 100 characters.
  - Use blank lines to separate logical blocks of code.

- **Naming Conventions**
  - Class names should be written in UpperCamelCase.
  - Method names should be written in lowerCamelCase.
  - Constant names should be written in CONSTANT_CASE.

- **Comments**
  - Use Javadoc (`/** ... */`) for all public classes and methods.
  - Use block comments (`/* ... */`) inside methods and end-of-line comments (`// ...`) sparingly.

- **Declarations**
  - One declaration per line is encouraged.
  - Initialize variables where they are declared, unless the initialization depends on some computation.

- **Statements**
  - Use a single statement per line.
  - Use braces for all control structures, even single-line statements.

- **Whitespace**
  - Use a space after keywords (e.g., `if (condition)` not `if(condition)`).
  - No space between a method name and the parenthesis (`methodName(param)`).

- **Imports**
  - Import statements should be grouped with a single blank line between each group.
  - No wildcard imports; import only what is needed.

- **Programming Practices**
  - Prefer dependency injection over static methods.
  - Avoid redundant initialization (e.g., `boolean flag = false;` is preferred over `boolean flag; flag = false;`).

## 💼 Hiring

We are a group of MMO enthusiasts running Voidara as a passion project. All positions are voluntary. Due to the nature of our work, new team members must sign an NDA and a copyright assignment. Therefore, we only hire individuals over the age of 18. If you are interested in joining our team and are willing to sign the necessary documents, please contact us via:

- Our [website](https://www.voidara.net) (currently down)
- Email at apply@voidara.net
- Our [Discord server](https://discord.voidara.net)
