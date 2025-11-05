# RWAV Bridge MCP

Control your Roon system using RWAV Bridge with an MCP‑aware client (Roo Code, VS Code, Copilot, ChatGPT Apps).

- Download RWAV Bridge: https://www.rwav-bridge.co.uk/downloads  
- Help (MCP): https://rwav-bridge.co.uk/mcp/

## Install

macOS / Linux (Homebrew)
```bash
brew tap calibress/rwav
brew install rwav-bridge-mcp
```

Windows / macOS / Linux (npm)
```bash
npm i -g @calibress/rwav-bridge-mcp
```

## Configure your MCP host

Paste this into your host’s MCP settings:

```json
{
  "mcpServers": {
    "rwav": {
      "transport": "stdio",
      "command": "rwav-bridge-mcp"
    }
  }
}
```

> Do not use a file path; the installer places `rwav-bridge-mcp` on your PATH.

## First run

1. Install & run RWAV Bridge on the same network as your Roon Core:  
   https://www.rwav-bridge.co.uk/downloads
2. Launch your MCP‑aware client; it will start `rwav-bridge-mcp` and discover the Bridge.

## Troubleshooting

- Bridge not found → ensure RWAV Bridge is running; then retry.  
  Downloads: https://www.rwav-bridge.co.uk/downloads
- Images → Local MCP uses the Bridge’s local resolver; Relay uses `https://cdn.rwav.app/`.
- More help: https://rwav-bridge.co.uk/mcp/

---

© Calibre Software Systems Ltd (trading as Calibress). RWAV Bridge MCP.
