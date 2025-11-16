
# Useful MCP Servers for Programmers

A curated list of Model Context Protocol (MCP) servers that enhance development workflows and productivity.

## 📋 Table of Contents

- [What is MCP?](#what-is-mcp)
- [Development Tools](#development-tools)
- [Database & Data Management](#database--data-management)
- [API & Web Services](#api--web-services)
- [File & System Operations](#file--system-operations)
- [Development Utilities](#development-utilities)
- [Documentation & Knowledge](#documentation--knowledge)
- [Monitoring & Analytics](#monitoring--analytics)
- [Cloud Services](#cloud-services)
- [Communication & Collaboration](#communication--collaboration)
- [Specialized Tools](#specialized-tools)
- [Getting Started](#getting-started)
- [Best Practices](#best-practices)
- [Resources](#resources)

---

## What is MCP?

Model Context Protocol (MCP) is an open protocol that standardizes how applications provide context to LLMs. It enables AI assistants to securely access data and tools through a common interface.

**Key Benefits:**
- 🔌 Standardized integration with AI tools
- 🔒 Secure access to external resources
- 🚀 Enhanced AI capabilities through tool use
- 🔄 Reusable server implementations

---

## Development Tools

### **GitHub MCP Server**
- **Purpose**: Interact with GitHub repositories, issues, PRs, and code
- **Features**:
  - Repository management (create, fork, clone)
  - Issue and PR creation/management
  - Code search and file operations
  - Branch and commit management
  - CI/CD workflow monitoring
- **Installation**: `npm install @modelcontextprotocol/server-github`
- **Configuration**:
```json
  {
    "github": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-github"],
      "env": {
        "GITHUB_TOKEN": "your-github-token"
      }
    }
  }
```
- **Use Cases**: Automating GitHub workflows, code reviews, project management

### **Git MCP Server**
- **Purpose**: Local Git repository operations
- **Features**:
  - View diffs and logs
  - Commit changes with AI-generated messages
  - Branch management
  - Repository status and history
- **Installation**: `npm install @modelcontextprotocol/server-git`
- **Use Cases**: Version control automation, commit message generation, repository analysis

### **GitLab MCP Server**
- **Purpose**: Interact with GitLab repositories and pipelines
- **Features**:
  - Repository operations
  - CI/CD pipeline management
  - Issue tracking
  - Merge request handling
- **Use Cases**: GitLab workflow automation, DevOps tasks

---

## Database & Data Management

### **PostgreSQL MCP Server**
- **Purpose**: Query and manage PostgreSQL databases
- **Features**:
  - Execute SQL queries
  - Database schema inspection
  - Data analysis and reporting
  - Transaction management
- **Installation**: `npm install @modelcontextprotocol/server-postgres`
- **Configuration**:
```json
  {
    "postgres": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-postgres"],
      "env": {
        "POSTGRES_CONNECTION_STRING": "postgresql://user:password@localhost:5432/dbname"
      }
    }
  }
```
- **Use Cases**: Database querying, schema exploration, data analysis

### **SQLite MCP Server**
- **Purpose**: Interact with SQLite databases
- **Features**:
  - Query execution
  - Database inspection
  - Lightweight data storage
  - No server setup required
- **Installation**: `npm install @modelcontextprotocol/server-sqlite`
- **Use Cases**: Local database management, testing, prototyping

### **MySQL MCP Server**
- **Purpose**: MySQL database operations
- **Features**:
  - Query execution
  - Schema management
  - Data manipulation
  - Performance analysis
- **Use Cases**: MySQL database administration and development

---

## API & Web Services

### **Fetch MCP Server**
- **Purpose**: Make HTTP requests to APIs
- **Features**:
  - GET, POST, PUT, DELETE requests
  - Header customization
  - Response parsing
  - Error handling
- **Installation**: `npm install @modelcontextprotocol/server-fetch`
- **Use Cases**: API testing, web scraping, integration testing

### **Puppeteer MCP Server**
- **Purpose**: Browser automation and web scraping
- **Features**:
  - Page navigation
  - Screenshot capture
  - Form interaction
  - Content extraction
  - JavaScript execution
- **Installation**: `npm install @modelcontextprotocol/server-puppeteer`
- **Use Cases**: End-to-end testing, web scraping, automation, PDF generation

### **Playwright MCP Server**
- **Purpose**: Cross-browser automation
- **Features**:
  - Multi-browser testing (Chrome, Firefox, Safari)
  - Parallel execution
  - Network interception
  - Mobile emulation
- **Use Cases**: E2E testing, browser automation, quality assurance

---

## File & System Operations

### **Filesystem MCP Server**
- **Purpose**: File system operations
- **Features**:
  - Read/write files
  - Directory operations
  - File search and filtering
  - Permission management
- **Installation**: `npm install @modelcontextprotocol/server-filesystem`
- **Configuration**:
```json
  {
    "filesystem": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-filesystem", "/path/to/allowed/directory"]
    }
  }
```
- **Use Cases**: File management, code generation, log analysis

### **Docker MCP Server**
- **Purpose**: Docker container and image management
- **Features**:
  - Container lifecycle management
  - Image operations (build, push, pull)
  - Network and volume management
  - Container logs and stats
- **Use Cases**: DevOps automation, container orchestration, development environments

---

## Development Utilities

### **Slack MCP Server**
- **Purpose**: Slack workspace integration
- **Features**:
  - Send messages to channels/users
  - Channel management
  - User operations
  - File sharing
- **Installation**: `npm install @modelcontextprotocol/server-slack`
- **Use Cases**: Team notifications, workflow automation, incident management

### **Google Drive MCP Server**
- **Purpose**: Google Drive file management
- **Features**:
  - File upload/download
  - Search documents
  - Share management
  - Folder operations
- **Use Cases**: Documentation management, file sharing, collaboration

### **Google Maps MCP Server**
- **Purpose**: Location and mapping services
- **Features**:
  - Geocoding and reverse geocoding
  - Route planning
  - Place search
  - Distance calculations
- **Use Cases**: Location-based applications, delivery routing, geographic data

---

## Documentation & Knowledge

### **Memory MCP Server**
- **Purpose**: Persistent knowledge storage for AI assistants
- **Features**:
  - Store and retrieve context
  - Knowledge graph creation
  - Long-term memory across sessions
  - Entity relationship tracking
- **Installation**: `npm install @modelcontextprotocol/server-memory`
- **Use Cases**: Maintaining context across sessions, knowledge management, personalization

### **Brave Search MCP Server**
- **Purpose**: Web search capabilities
- **Features**:
  - Web search
  - Result filtering
  - Privacy-focused
  - No tracking
- **Use Cases**: Research, documentation lookup, current information retrieval

---

## Monitoring & Analytics

### **Sentry MCP Server**
- **Purpose**: Error tracking and monitoring
- **Features**:
  - Error querying
  - Issue management
  - Performance monitoring
  - Release tracking
- **Use Cases**: Bug tracking, production monitoring, debugging

### **Prometheus MCP Server**
- **Purpose**: Metrics and monitoring
- **Features**:
  - Query metrics
  - Alert management
  - Time-series data
  - Dashboard integration
- **Use Cases**: System monitoring, performance analysis, alerting

---

## Cloud Services

### **AWS KB Retrieval MCP Server**
- **Purpose**: AWS knowledge base integration
- **Features**:
  - Document retrieval
  - Semantic search
  - AWS service integration
  - Context-aware responses
- **Use Cases**: Documentation access, knowledge management, AWS support

### **Google Cloud Platform MCP Server**
- **Purpose**: GCP service management
- **Features**:
  - Resource management
  - Service operations
  - Cloud infrastructure monitoring
  - Cost analysis
- **Use Cases**: Cloud automation, infrastructure management

### **Azure MCP Server**
- **Purpose**: Microsoft Azure service integration
- **Features**:
  - Resource management
  - Azure DevOps integration
  - Service monitoring
  - Deployment automation
- **Use Cases**: Azure cloud operations, DevOps workflows

---

## Communication & Collaboration

### **Linear MCP Server**
- **Purpose**: Linear issue tracking integration
- **Features**:
  - Issue creation/management
  - Project tracking
  - Team collaboration
  - Sprint planning
- **Use Cases**: Project management, sprint planning, bug tracking

### **Asana MCP Server**
- **Purpose**: Asana task management
- **Features**:
  - Task operations
  - Project management
  - Workflow automation
  - Team coordination
- **Use Cases**: Task tracking, project coordination

### **Jira MCP Server**
- **Purpose**: Jira issue and project management
- **Features**:
  - Issue CRUD operations
  - Sprint management
  - Custom field handling
  - Workflow automation
- **Use Cases**: Agile project management, bug tracking, sprint planning

---

## Specialized Tools

### **Exa MCP Server**
- **Purpose**: Advanced web search and data extraction
- **Features**:
  - Semantic search
  - Content extraction
  - Research tools
  - AI-powered results
- **Use Cases**: Research, competitive analysis, data gathering

### **Sequential Thinking MCP Server**
- **Purpose**: Dynamic problem-solving through thought sequences
- **Features**:
  - Step-by-step reasoning
  - Thought process tracking
  - Reflective problem-solving
  - Complex task breakdown
- **Use Cases**: Complex problem solving, debugging, architectural decisions

---

## Getting Started

### Prerequisites

- Node.js 18+ installed
- Claude Desktop or compatible MCP client
- API keys/tokens for services you want to use

### Installation

Most MCP servers can be installed via npm:
```bash
npm install @modelcontextprotocol/server-[name]
```

Or use them directly with npx (no installation required):
```bash
npx @modelcontextprotocol/server-[name]
```

### Configuration

Configure MCP servers in your Claude Desktop config file:

**MacOS**: `~/Library/Application Support/Claude/claude_desktop_config.json`

**Windows**: `%APPDATA%\Claude\claude_desktop_config.json`

**Linux**: `~/.config/Claude/claude_desktop_config.json`

### Example Configuration
```json
{
  "mcpServers": {
    "github": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-github"],
      "env": {
        "GITHUB_TOKEN": "ghp_your_token_here"
      }
    },
    "filesystem": {
      "command": "npx",
      "args": [
        "-y",
        "@modelcontextprotocol/server-filesystem",
        "/Users/username/projects"
      ]
    },
    "postgres": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-postgres"],
      "env": {
        "POSTGRES_CONNECTION_STRING": "postgresql://user:pass@localhost:5432/db"
      }
    },
    "slack": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-slack"],
      "env": {
        "SLACK_BOT_TOKEN": "xoxb-your-token",
        "SLACK_TEAM_ID": "T1234567890"
      }
    }
  }
}
```

### Testing Your Setup

1. Save your configuration file
2. Restart Claude Desktop
3. Check the MCP status in Claude Desktop settings
4. Try a simple command like: "List my GitHub repositories"

---

## Best Practices

### Security

1. **Environment Variables**: Always use environment variables for API keys and tokens
2. **Token Permissions**: Use the minimum required permissions for access tokens
3. **Never Commit Secrets**: Don't commit config files with secrets to version control
4. **Regular Rotation**: Rotate API keys and tokens regularly
5. **Read-Only Mode**: Use read-only modes when possible (e.g., GitHub read-only)

### Performance

1. **Scope Limitations**: Limit filesystem and database access to necessary directories/databases only
2. **Connection Pooling**: Configure proper connection pooling for database servers
3. **Caching**: Enable caching where available to reduce API calls
4. **Rate Limiting**: Be aware of API rate limits and implement backoff strategies

### Development

1. **Testing**: Test MCP servers in development before production use
2. **Updates**: Keep MCP servers updated for latest features and security patches
3. **Monitoring**: Monitor MCP server logs for errors and issues
4. **Documentation**: Document your MCP server configurations for team members
5. **Version Control**: Track your MCP configuration in version control (without secrets)

---

## Troubleshooting

### Common Issues

**Server not connecting:**
- Check if the server package is installed
- Verify your configuration syntax
- Ensure API keys are valid and have proper permissions
- Check Claude Desktop logs for error messages

**Permission errors:**
- Verify filesystem paths are accessible
- Check API token permissions
- Ensure database credentials are correct

**Slow performance:**
- Check network connectivity
- Verify API rate limits aren't being exceeded
- Consider using local caching

---

## Resources

### Official Documentation
- [Model Context Protocol Documentation](https://modelcontextprotocol.io)
- [MCP Specification](https://spec.modelcontextprotocol.io)
- [MCP GitHub Repository](https://github.com/modelcontextprotocol)
- [Claude Desktop Documentation](https://docs.anthropic.com/claude/docs)

### Community
- [MCP GitHub Discussions](https://github.com/modelcontextprotocol/discussions)
- [Anthropic Community Forum](https://community.anthropic.com)

### Learning Resources
- [Building MCP Servers Guide](https://modelcontextprotocol.io/docs/building-servers)
- [MCP Server Examples](https://github.com/modelcontextprotocol/servers)
- [MCP Best Practices](https://modelcontextprotocol.io/docs/best-practices)

---

## Contributing

Contributions are welcome! If you'd like to add a new MCP server to this list or improve existing documentation:

1. Fork this repository
2. Create a new branch (`git checkout -b add-new-server`)
3. Make your changes
4. Submit a pull request

### Contribution Guidelines

- Ensure the MCP server is publicly available
- Include installation instructions
- Provide example configuration
- Describe real-world use cases
- Keep descriptions concise and clear

---

## License

This list is provided as-is for informational purposes. Individual MCP servers have their own licenses.

---

## Acknowledgments

Thanks to:
- Anthropic for creating the Model Context Protocol
- The MCP community for developing these amazing servers
- Contributors who help maintain this list

---

**Last Updated**: November 2025

**Maintained by**: [@Arifns18](https://github.com/Arifns18)

---

## Quick Reference

| Category | Server | Best For |
|----------|--------|----------|
| Version Control | GitHub | Repository management, CI/CD |
| Version Control | Git | Local repository operations |
| Database | PostgreSQL | Production databases |
| Database | SQLite | Local/embedded databases |
| API Testing | Fetch | HTTP requests |
| Browser Automation | Puppeteer | Web scraping, testing |
| File Operations | Filesystem | File management |
| Containers | Docker | Container management |
| Team Communication | Slack | Notifications, collaboration |
| Knowledge | Memory | Context persistence |
| Monitoring | Sentry | Error tracking |
| Cloud | AWS/Azure/GCP | Cloud infrastructure |
| Project Management | Linear/Jira | Task tracking |

---

**⭐ Star this repo if you find it helpful!**
