# Home Assistant MCP Server

Model Context Protocol (MCP) Server for Home Assistant  
Provides SSE‑based tools to inspect and optimize your automations, scripts, scenes, and helpers.

## Features

- **SSE transport** with API‑Key authentication  
- **Tools**: `get_automations`, `get_scripts`, `get_scenes`, `get_helpers`  
- **Optimization** via `recommend_optimizations`

## Setup

1. **Clone** and `cd` into this repo  
2. Copy `.env.example` → `.env` and fill in values  
3. `npm install`  
4. `npm run build`  
5. `npm start`

Server runs at `http://localhost:${PORT}/sse` (default 8080).  
Use `X-API-Key` header to authenticate.

## Tools

- **get_automations** → list all automations  
- **get_scripts** → list all scripts  
- **get_scenes**  → list all scenes  
- **get_helpers** → list all helpers  
- **recommend_optimizations** → simple recommendations based on fetched data

MIT License
