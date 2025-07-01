# MCP Servers for Claude Desktop

## Overview

This repository contains a collection of servers that provide various tools and capabilities. They are designed to be run and managed by an environment like Claude Desktop, rather than being run manually by an end-user.

This document provides a brief overview of each server and development setup instructions.

## Servers

### Sequential Thinking Server
This server helps with complex problem-solving by breaking tasks down into steps. It's built with Node.js and TypeScript.

### MCP Neo4j Cypher
This server is designed to interact with a Neo4j graph database using the Cypher query language. It is a Python-based server.

### Data Gen
This server is a tool for generating data for your projects. It is a Python-based server.

## Development Setup

If you are developing these servers, you'll need to install their dependencies.

### Prerequisites

Make sure you have the following installed on your system:
-   **Node.js**: We recommend downloading the LTS version from the [official Node.js website](https://nodejs.org/).
-   **Python**: You can get it from the [official Python website](https://www.python.org/downloads/).
-   **`uv`**: A fast Python package installer. After installing Python, run `pip install uv` in your terminal.

### Installing Server Dependencies

From the root of the repository, run the following commands for each server you are working on.

**Sequential Thinking Server**
```bash
cd sequential-thinking-server
npm install
npm run build
```

**MCP Neo4j Cypher**
```bash
cd mcp-neo4j-cypher
uv pip install .
```

**Data Gen**
```bash
cd data-gen
pip install -r requirements.txt
```

## Contributing

Please feel free to open an issue to report a problem or suggest an improvement.