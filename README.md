# MCP Proxy Hub

MCP Proxy Hub is a comprehensive solution for managing multiple Model Context Protocol (MCP) servers through a single unified endpoint. It allows AI assistants like Cursor, Claude Desktop, and other MCP-compatible tools to access a wide range of capabilities through a centralized proxy.

![MCP Proxy Hub](https://github.com/yourusername/mcp-proxy-hub/asseures

- **Single Endpoint**: Connect AI tools to dozens of MCP servers through one proxy
- **Web Dashboard**: Intuitive UI for managing MCP servers
- **Server Discovery**: Easily discover and install MCP servers from repositories
- **Process Management**: Start, stop, and monitor MCP server processes
- **Real-time Monitoring**: View logs and performance metrics
- **Docker Deployment**: Simple containerized deployment

## Why Use MCP Proxy Hub?

Managing multiple MCP servers with AI assistants typically requires configuring each server individually in every tool. MCP Proxy Hub eliminates this complexity by:

- Providing a single connection point for all AI tools
- Centralizing server management and configuration
- Simplifying discovery and installation of new capabilities
- Offering real-time monitoring and logs
- Standardizing deployment through Docker

## Quick Start

### Using Docker (Recommended)

```bash
# Clone the repository
git clone https://github.com/yourusername/mcp-proxy-hub.git
cd mcp-proxy-hub

# Start the container
docker-compose up -d

# Access the UI
open http://localhost:8080
```

### Configure in AI Tools

In Cursor IDE:
1. Open Settings > MCP Servers
2. Add a new server with URL `http://localhost:3008`

In Claude Desktop:
1. Open Settings > MCP Servers
2. Add a new server with URL `http://localhost:3008`

## Architecture

MCP Proxy Hub consists of several components:

- **Proxy Server**: Routes MCP requests to appropriate backend servers
- **Server Manager**: Handles server lifecycle and configuration
- **API Server**: Provides RESTful endpoints for management
- **Web UI**: React-based interface for configuration and monitoring
- **Database**: Stores server configurations and logs

## Development

### Prerequisites

- Node.js 16+
- npm or yarn
- Git

### Setup

```bash
# Clone the repository
git clone https://github.com/yourusername/mcp-proxy-hub.git
cd mcp-proxy-hub

# Install dependencies
npm install

# Start development servers
npm run dev:proxy  # Start proxy server
npm run dev:api    # Start API server
npm run dev:ui     # Start UI development server
```

### Project Structure

```
mcp-proxy-hub/
├── src/
│   ├── proxy/       # MCP proxy implementation
│   ├── server/      # Server management
│   ├── api/         # REST API
│   ├── db/          # Database layer
│   ├── ui/          # React frontend
│   ├── types/       # TypeScript definitions
│   └── main.ts      # Application entry point
├── docker/          # Docker configuration
└── ...
```

## Available MCP Servers

MCP Proxy Hub integrates with repositories like [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) to provide access to a wide range of capabilities including:

- GitHub integration
- Web browser automation
- File system access
- API connections
- Database tools
- And many more

## Deployment Options

### Docker (Recommended)

Use the provided Docker configuration for a containerized deployment:

```bash
docker-compose up -d
```

### Manual Deployment

For advanced users who want to customize their setup:

```bash
# Build the application
npm run build

# Start the server
npm start
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [Model Context Protocol](https://github.com/anthropics/model-context-protocol) - For the protocol specification
- [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - For the collection of MCP servers
- [adamwattis/mcp-proxy-server](https://github.com/adamwattis/mcp-proxy-server) - For inspiration
- [zueai/mcp-manager](https://github.com/zueai/mcp-manager) and other MCP management tools

---

**Note**: MCP Proxy Hub is currently in active development. Please report any issues you encounter.

---
Réponse de Perplexity: pplx.ai/share