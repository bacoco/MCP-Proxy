# Main Application

Create the main application entry point with the following features:

1. Application Bootstrap:
   - Initialize database connection
   - Create server manager instance
   - Start proxy server
   - Start API server
   - Set up signal handlers for graceful shutdown

2. Configuration:
   - Load configuration from environment variables
   - Set default values for missing configuration
   - Validate configuration values
   - Log configuration (without sensitive values)

3. Logging:
   - Configure logging with proper levels
   - Add request ID tracking
   - Include timestamps and log levels
   - Support different output formats (JSON, text)

4. Error Handling:
   - Set up global error handlers
   - Log uncaught exceptions
   - Implement graceful shutdown
   - Provide meaningful error messages

5. Monitoring:
   - Track basic metrics (requests, errors, etc.)
   - Implement health check endpoint
   - Add performance monitoring
   - Include resource usage tracking

The main application should be robust, handling startup errors gracefully, and should support proper shutdown when terminated.
