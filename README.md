# n8n-node-MCP-Server
A universal agentic interface connecting an AI to a N8N flow via a MCP Server

The proof of concept:

1) Use a AI, in this case Claude Code
2) Create a MCP server to expose N8N MCP endpoints
3) create a flow that can interact with claude

Requirements:
- N8N: Currently only works with n8n@1.116.1 installed in your docker.
- VS Code with Claude code installed -> or similar enviroment to support Claude Code.
- MCP-Server.



Within Claude Code
-> Type: what tools do I have acceess too

Claude Code response:

Based on the MCP tools available, I have access to these two N8N MCP tools:
mcp__n8n__webhook-trigger - Trigger an N8N webhook with custom data
Required parameter: data (object) - Data to send to the webhook
mcp__n8n__http-request - Make HTTP requests through N8N
Required parameter: url (string) - Target URL
Optional parameter: method (string) - HTTP method (GET, POST, PUT, DELETE, etc.)


-> Type: mcp__n8n__http-request to https://books.toscrape.com/ using get then create a csv flie of all the details of all the books on the first two pages of the site (authur, title, price, image link)
