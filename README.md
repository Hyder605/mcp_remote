# mcp_remote

## Overview

This repository contains two MCP (Model Context Protocol) server implementations:

1. **main.py** - Async MCP server for expense tracking using aiosqlite
2. **proxy.py** - MCP proxy for connecting to a remote FastMCP Cloud server

## Contents

### Files:
- **main.py**: Async MCP server with expense tracking functionality using aiosqlite
- **proxy.py**: MCP proxy client for connecting to remote FastMCP Cloud servers
- **categories.json**: JSON file defining expense categories
- **expenses.db**: SQLite database file (stored in temp directory)
- **pyproject.toml**: Python project configuration
- **uv.lock**: Dependency lock file

## Features

### main.py:
- Async expense tracking MCP server
- Uses aiosqlite for async database operations
- Stores database in system temp directory
- Includes database initialization and schema creation

### proxy.py:
- MCP proxy for remote server connections
- Connects to FastMCP Cloud servers
- Standard MCP proxy implementation

## Usage

### Running the servers:

```bash
# Run the async expense tracker
python main.py

# Run the remote proxy
python proxy.py
```

### main.py Features:
- Async database operations with aiosqlite
- Temporary database storage
- Basic expense tracking functionality

### proxy.py Features:
- Remote server connection proxy
- Standard MCP proxy implementation

## Dependencies
- Python 3.9+
- fastmcp library
- aiosqlite for async database operations

## Note

This is a **learning/experimental** repository for exploring:
- Async MCP server implementation with aiosqlite
- MCP proxy patterns for remote server connections
- Different approaches to MCP server architecture

## Owner

Hyder