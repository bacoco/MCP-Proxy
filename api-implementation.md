# API Implementation

Create a RESTful API with Express.js that provides the following endpoints:

1. Server Management:
   - GET /api/servers - List all servers
   - POST /api/servers - Add new server
   - GET /api/servers/:id - Get server details
   - PUT /api/servers/:id - Update server
   - DELETE /api/servers/:id - Remove server
   - POST /api/servers/:id/start - Start server
   - POST /api/servers/:id/stop - Stop server
   - GET /api/servers/:id/logs - Get server logs

2. Discovery:
   - GET /api/discovery/sources - List available sources
   - GET /api/discovery/servers - List available servers
   - POST /api/discovery/install/:id - Install server

3. System:
   - GET /api/system/status - Get system status
   - GET /api/system/metrics - Get performance metrics
   - GET /api/health - Health check endpoint

4. Authentication (if implemented):
   - POST /api/auth/login - Log in
   - POST /api/auth/logout - Log out
   - GET /api/auth/status - Get auth status

5. Include the following middleware:
   - Request validation
   - Authentication/authorization
   - Error handling
   - CORS configuration
   - Rate limiting
   - Request logging

The API should follow REST best practices, with proper status codes, response formats, and error handling.
