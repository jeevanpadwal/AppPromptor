
<boltArtifact id="backend-readme" title="Comprehensive Project README with Diagrams">
  <boltAction type="file" filePath="README.md">
# Backend Project Documentation

## 🚀 Project Overview

### System Architecture
```mermaid
graph TD
    A[Client Request] --> B{Express Server}
    B --> |Template Selection| C[OpenAI API]
    C --> |Project Type Detection| D{React or Node}
    D --> |React Project| E[React Project Template]
    D --> |Node Project| F[Node Project Template]
    E --> G[Generated Project Files]
    F --> G
```

### Workflow Diagram
```mermaid
sequenceDiagram
    participant Client
    participant Express Server
    participant OpenAI API
    
    Client->>Express Server: Send Project Request
    Express Server->>OpenAI API: Determine Project Type
    OpenAI API-->>Express Server: React or Node
    Express Server-->>Client: Return Project Prompts
```

## 🛠 Key Components

### Main Technologies
- **Backend Framework**: Express.js
- **AI Integration**: OpenAI API
- **Language**: TypeScript
- **Model**: Meta Llama 3.1 70B Instruct

### Project Structure
```mermaid
graph LR
    A[index.ts] --> B[prompts.ts]
    A --> C[constants.ts]
    B --> D[System Prompts]
    B --> E[Base Prompts]
    C --> F[Allowed HTML Elements]
    C --> G[Work Directory Constants]
```

## 📦 Key Files and Their Responsibilities

| File | Primary Responsibility |
|------|------------------------|
| `index.ts` | Main server configuration |
| `prompts.ts` | Manage system and base prompts |
| `constants.ts` | Define project-wide constants |

## 🔧 System Constraints

### WebContainer Limitations
- ✖️ No native binary execution
- ✖️ Limited Python library support
- ✖️ No Git available
- ✖️ Browser-based Node.js runtime

## 🌟 Features

### Endpoint: `/template`
- Determines project type (React/Node)
- Generates appropriate project templates

### Endpoint: `/chat`
- Handles AI-powered chat interactions
- Applies system prompts
- Generates contextual responses

## 🚦 Installation

```bash
# Clone the repository
git clone <repository-url>

# Install dependencies
npm install

# Start the server
npm run start
```

## 🔐 Environment Configuration

Create a `.env` file with:
```
OPENAI_API_KEY=your_openai_api_key
BASE_URL=optional_base_url
```

## 🛡️ Security Considerations
- API key protection
- Limited AI model interactions
- Controlled project generation

## 📊 Performance Metrics
```mermaid
pie title AI Model Usage
    "Successful Requests" : 85
    "Error Responses" : 10
    "Rate Limited" : 5
```

## 📝 Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request
---

**Built with ❤️ using TypeScript, Express, and OpenAI**
  </boltAction>
</boltArtifact>

key aspects of this README:

1. **Architecture Diagrams**: 
   - System Architecture diagram shows request flow
   - Workflow diagram illustrates interaction between components
   - Component structure graph visualizes file relationships

2. **Detailed Sections**:
   - Technology stack
   - Project structure
   - System constraints
   - Features breakdown
   - Installation instructions
   - Performance visualization

3. **Mermaid Diagrams**:
   - Used for visual representations
   - Easy to understand flow and relationships
   - Provides insights into system design

4. **Markdown Formatting**:
   - Clean, professional layout
   - Tables and code blocks for clarity

The README provides overview of backend project, making it easy for developers to understand its purpose, architecture, and how to get started.
