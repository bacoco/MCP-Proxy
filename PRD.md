# Cursor AI Implementation Prompts

## 1. Initial Project Setup

```
Based on the project-structure.md file, set up the initial project structure with package.json, tsconfig.json, and the basic folder structure. Initialize a TypeScript Node.js project with Express.js for the API server, and configure ESLint and Prettier. Install all required dependencies for a proxy server, database, and React frontend.
```

## 2. MCP Protocol Types

```
Using the specifications in mcp-types.md, implement the core TypeScript interfaces and types for the MCP protocol. Create all the required types including MCPRequest, MCPResponse, MCPTool, MCPParameter, MCPServerConfig, and necessary enums like TransportType and ServerStatus. Place these in the src/types/index.ts file.
```

## 3. Database Layer

```
Implement the SQLite database layer as specified in database-implementation.md. Create the database connection, models, and CRUD operations for server configurations and logs. Include migration support for schema changes. Focus on implementing the core database functionality in src/db/index.ts and related files.
```

## 4. Server Manager

```
Based on server-manager.md, implement the ServerManager class in src/server/manager.ts that can start, stop, and monitor MCP server processes. Include functionality to capture stdout/stderr, manage configurations, and handle process lifecycle events. Make sure it integrates with the database layer we've already implemented.
```

## 5. MCP Proxy Core

```
Implement the core MCP proxy functionality specified in proxy-implementation.md. Create the main router in src/proxy/router.ts that can accept MCP requests, route them to appropriate backend servers, and aggregate responses. Support both stdio and SSE transports, and include proper error handling.
```

## 6. API Routes and Controllers

```
Using the specifications in api-implementation.md, implement the Express.js API endpoints in the src/api directory. Create controllers for server management, discovery, and system status. Implement proper route handlers, middleware for validation, and error handling. Ensure the API integrates with the ServerManager we've already implemented.
```

## 7. Server Discovery Service

```
Implement the server discovery service described in server-manager.md. Create functionality to fetch available MCP servers from repositories like awesome-mcp-servers, parse metadata, and prepare installation instructions. Implement this in src/server/discovery.ts and ensure it integrates with the API we've already built.
```

## 8. Application Entry Point

```
Based on main-application.md, implement the main application entry point in src/main.ts. Set up the initialization sequence that starts the database, server manager, proxy server, and API server. Include configuration loading, logging setup, and signal handlers for graceful shutdown.
```

## 9. React UI Components

```
Using the specifications in ui-implementation.md, implement the core React components for the UI. Start with the basic layout including the dashboard, server list, and server detail views. Create the Redux store structure and API client services. Focus on the main UI functionality in the src/ui directory.
```

## 10. Docker Configuration

```
Based on docker-config.md, create the Dockerfile and docker-compose.yml files in the docker directory. Implement a multi-stage build process, proper volume configuration, and port mapping. Ensure the Docker configuration follows best practices for security and performance.
```

## 11. Unit and Integration Tests

```
Implement the testing suite described in testing-suite.md. Create unit tests for core components like the ServerManager, proxy router, and API controllers. Add integration tests for database operations and API endpoints. Set up Jest configuration and test utilities.
```

## 12. Complete End-to-End Flow

```
Connect all the components we've implemented to create a complete end-to-end flow. Ensure the proxy server can route requests to backend servers managed by the ServerManager, the API server can control these servers, and the UI can interact with the API. Fix any integration issues and ensure proper error handling throughout the application.
```

## 13. Performance Optimization

```
Review the implemented code and optimize performance for the MCP proxy server. Focus on minimizing latency for request routing, efficient tool aggregation, and proper resource management for spawned processes. Add caching where appropriate and ensure efficient database queries.
```

## 14. Security Review

```
Enhance the security of the application by implementing proper authentication for the API, secure handling of server credentials, input validation, and protection against common vulnerabilities. Review Docker configuration for security best practices and ensure proper error handling that doesn't leak sensitive information.
```

## 15. Final Integration and Polishing

```
Connect the React UI to the backend API, implement real-time updates with WebSockets, and ensure smooth user experience for server management. Add final polishing touches like improved error messages, loading states, and confirmation dialogs. Ensure consistent styling and responsive design throughout the UI.
```
