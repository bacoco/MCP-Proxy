# Docker Configuration

Create Docker configuration files with the following requirements:

1. Dockerfile:
   - Use multi-stage build for optimization
   - Base on Node.js Alpine for small footprint
   - Install only production dependencies
   - Set up proper working directory
   - Copy only necessary files
   - Build both backend and frontend
   - Configure environment variables
   - Set up health check
   - Expose necessary ports (3008 for MCP, 8080 for UI)
   - Create volume mount points for persistence
   - Set up non-root user for security

2. docker-compose.yml:
   - Define service for MCP Proxy Hub
   - Configure port mappings
   - Set up volume mounts
   - Define environment variables
   - Add restart policy
   - Set resource limits
   - Add healthcheck configuration
   - Configure logging

3. Include instructions for:
   - Building the image
   - Running the container
   - Persisting data
   - Updating the application
   - Troubleshooting common issues

The Docker configuration should follow best practices for security, performance, and maintainability.
