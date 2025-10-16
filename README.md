
# Azure Function App - Hello World

This is a simple Azure Function App with an HTTP trigger that returns a hello world message.

## Local Development Setup

1. Install Azure Functions Core Tools:
   ```bash
   npm install -g azure-functions-core-tools@4 --unsafe-perm true
   ```

2. Install Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run locally:
   ```bash
   func start
   ```

4. Test the function:
   ```bash
   curl http://localhost:7071/api/HttpTrigger?name=World
   ```

## Deployment

The function app is configured to deploy to Azure subscription: 3ccf6ed9-c22c-48bc-b26c-fd633fb1196c

## Function Endpoints

- **HttpTrigger**: HTTP GET/POST endpoint that accepts a `name` parameter
  - URL: `https://your-function-app.azurewebsites.net/api/HttpTrigger`
  - Query parameter: `name` (optional)
  - Returns: Personalized greeting or default message