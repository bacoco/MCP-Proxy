# MCP Type Definitions

Create TypeScript interfaces for the MCP protocol with the following requirements:

1. Define the core MCP protocol types including:
   - MCPRequest: The structure of incoming requests
   - MCPResponse: The structure of outgoing responses
   - MCPError: Error format
   - MCPTool: Tool definition
   - MCPParameter: Parameter definition for tools
   - MCPServerConfig: Configuration for an MCP server

2. Include proper JSDoc comments for all interfaces

3. Define type-safe enums for:
   - TransportType: 'stdio' | 'sse'
   - ServerStatus: 'starting' | 'running' | 'stopping' | 'stopped' | 'error'
   - ParameterType: standard JSON Schema types

4. Create utility types for:
   - Partial configurations
   - Request validation
   - Response formatting

5. Ensure the types are compatible with the MCP protocol specification

The types should be comprehensive enough to type the entire application, from proxy server to UI components. Use generics where appropriate for flexibility.
