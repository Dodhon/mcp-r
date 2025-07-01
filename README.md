# MCP Servers for Claude Desktop

## Overview

This repository contains a collection of servers that provide various tools and capabilities. They are designed to be run and managed by an environment like Claude Desktop, rather than being run manually by an end-user.

This document guides you through setting up a full development environment and provides an overview of the servers.

### Included Servers

*   **Sequential Thinking Server**: Helps with complex problem-solving by breaking tasks down into steps. It's built with Node.js and TypeScript.
*   **MCP Neo4j Cypher**: Interacts with a Neo4j graph database using the Cypher query language. It is a Python-based server.
*   **Data Gen**: A tool for generating data for your projects. It is a Python-based server.

## Full Environment Setup

Follow these steps if you are setting up a new machine for development.

### 1. Install Visual Studio Code

A code editor is required to work with this project. We recommend VS Code.

1.  Go to the [official VS Code website](https://code.visualstudio.com/).
2.  Download and run the installer for your operating system.

### 2. Set Up Claude Desktop

These servers are designed to be managed by Claude Desktop. For instructions on how to install and configure it, please see the separate setup guide.

**Note:** Using MCPs with Claude Desktop requires a Claude Pro subscription.

### 3. Install Development Tools

You'll need Node.js and Python to develop the servers.

*   **Node.js**: Download the LTS version from the [official Node.js website](https://nodejs.org/).
*   **Python**: Get the latest version from the [official Python website](https://www.python.org/downloads/).
*   **`uv`**: A fast Python package installer. After installing Python, open your terminal and run `pip install uv`.

### 4. Install Server Dependencies

Once your environment is set up, you can install the dependencies for each server. From the root of this project in your terminal, run the relevant commands:

**For the Sequential Thinking Server:**
```bash
cd sequential-thinking-server
npm install
npm run build
```

**For the MCP Neo4j Cypher Server:**
```bash
cd mcp-neo4j-cypher
uv pip install .
```

**For the Data Gen Server:**
```bash
cd data-gen
pip install -r requirements.txt
```

## Contributing

Please feel free to open an issue to report a problem or suggest an improvement.