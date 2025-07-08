# 🤖 AA Kit: Agent As Everything

<div align="center">
  <img src="https://img.shields.io/badge/Status-Coming%20Soon-orange?style=for-the-badge" alt="Coming Soon" />
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" alt="MIT License" />
  <img src="https://img.shields.io/badge/Python-3.8+-green?style=for-the-badge" alt="Python 3.8+" />
</div>

<div align="center">
  <h3>🚀 One Agent, Many Forms</h3>
  <p><em>Your agent is a tool. Your agent is a server. Your agent is a function.<br/>
  With AA Kit, agents transcend categories.</em></p>
</div>

---

## 🌟 The Philosophy

> **"When you realize an agent can be a tool for another agent, and that tool is also an agent, you understand: agents are the universal primitive of AI."**

AA Kit isn't just another agent framework—it's a paradigm shift. We believe agents shouldn't be boxed into roles like "chatbot" or "assistant." Instead, agents are the **universal primitive** of AI systems, capable of being:

- 🔧 **Tools** for other agents
- 🌐 **Servers** via MCP protocol  
- ⚡ **Functions** that compose naturally
- 🏗️ **Building blocks** for AI ecosystems

## ✨ What Makes AA Kit Different

### 🎯 **Agent = Function**
```python
# Three parameters. Returns intelligence. No complexity.
agent = Agent(
    name="assistant",
    instruction="You are a helpful assistant", 
    model="gpt-4"
)
```

### 🌐 **Agent = Server**
```python
# Every agent exposes itself as an MCP server instantly
agent.serve_mcp()
# Now available at: http://localhost:8080/mcp
```

### 🔗 **Agent = Tool**
```python
# Pass one agent to another as a tool
writer = Agent(
    name="writer",
    instruction="You write articles",
    model="gpt-4",
    tools=[researcher_agent]  # Natural composition
)
```

### 🚀 **Agent = Production**
Rate limits, retries, caching, circuit breakers—not added later, but built into the constructor from day one.

## 🎨 Core Features

<table>
<tr>
<td width="33%">

### 🏗️ **Universal Composition**
Agents compose naturally because they're all the same primitive underneath. No special interfaces or adapters needed.

</td>
<td width="33%">

### 🌐 **MCP Native**
Every agent is automatically MCP-compatible. Zero configuration, instant interoperability with the entire MCP ecosystem.

</td>
<td width="33%">

### ⚡ **Production Ready**
Built-in rate limiting, retry logic, circuit breakers, and caching. Scale from prototype to production without refactoring.

</td>
</tr>
</table>

## 📊 By The Numbers

<div align="center">

| **3** | **0** | **∞** | **1** |
|-------|-------|-------|-------|
| Lines to Production | Config for MCP | Composition Depth | Universal Protocol |

</div>

## 🔮 Coming Soon

The open source release of AA Kit is being finalized. Here's what you can expect:

### 📦 **Core Package**
- Pure Python implementation
- Zero external dependencies for core functionality
- Support for OpenAI, Anthropic, and local models
- Built-in memory backends (Redis, SQLite, PostgreSQL)

### 🛠️ **Developer Experience**
- Rich CLI with interactive agent builder
- Hot-reloading for development
- Comprehensive debugging tools
- Extensive examples and tutorials

### 🌐 **MCP Ecosystem**
- Automatic server generation
- Client connection helpers
- Protocol validation and testing
- Community tool registry

### 📚 **Documentation**
- Comprehensive API reference
- Architecture deep-dives
- Production deployment guides
- Framework comparison analysis

## 🎯 Quick Preview

While we prepare the full release, here's a taste of the AA Kit experience:

```python
from aakit import Agent

# Create a research agent
researcher = Agent(
    name="researcher",
    instruction="You research topics thoroughly and provide detailed analysis",
    model="gpt-4"
)

# Create a writer that uses the researcher
writer = Agent(
    name="writer", 
    instruction="You write engaging articles based on research",
    model="claude-3",
    tools=[researcher]  # Composition magic
)

# Serve both as MCP servers
researcher.serve_mcp(port=8080)
writer.serve_mcp(port=8081)

# Now available to the entire MCP ecosystem!
```

## 🚀 Get Notified

Want to be among the first to build with AA Kit?

- ⭐ **Star this repo** to get notified when we launch
- 🐦 **Follow us** on [Twitter](https://twitter.com/aakit_ai) for updates
- 📧 **Join our mailing list** at [aakit.dev](https://aakit.dev)
- 💬 **Join our Discord** for early access discussions

## 🤝 Early Access

Interested in contributing or getting early access? We're looking for:

- 🏗️ **Framework developers** familiar with agent architectures
- 🧪 **Beta testers** building production AI systems  
- 📝 **Technical writers** passionate about developer experience
- 🎨 **UI/UX designers** for our developer tools

Reach out at [hello@aakit.dev](mailto:hello@aakit.dev)

## 🌟 The Vision

AA Kit represents a fundamental shift in how we think about AI agents:

> **Not as isolated applications, but as composable primitives that form the building blocks of intelligent systems.**

Every agent can be:
- A standalone application
- A tool for other agents  
- A server in a distributed system
- A function in a larger computation

This isn't just code—it's a new way of architecting AI.

## 📄 License

MIT License - see [LICENSE](LICENSE) for details.

---

<div align="center">
  <strong>🤖 Agent As Everything. Everything As Agent. 🤖</strong>
  <br/><br/>
  <em>The future of AI is composable.</em>
</div>
