# MCP Proxy Implementation

Create the core MCP proxy server with the following requirements:

1. Implement a server that can:
   - Accept MCP protocol requests
   - Route requests to appropriate backend servers
   - Aggregate responses
   - Handle errors gracefully

2. Support two transport mechanisms:
   - STDIO: For process-based communication
   - SSE: For HTTP-based communication

3. Create a router that can:
   - Map tool requests to appropriate backend servers
   - Maintain a registry of available tools
   - Handle tool conflicts (same name from different servers)

4. Implement tool aggregation logic that:
   - Combines tools from multiple servers
   - Preserves tool metadata
   - Handles version conflicts

5. Add proper error handling for:
   - Malformed requests
   - Server failures
   - Timeouts
   - Authentication failures

6. Include health checks for:
   - Backend server availability
   - Transport connectivity

The implementation should be efficient, handling requests with minimal latency, and should support both synchronous and asynchronous MCP tools.
