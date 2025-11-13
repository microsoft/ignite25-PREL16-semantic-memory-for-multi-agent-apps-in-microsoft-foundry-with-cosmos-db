<p align="center">
<img src="img/Banner-ignite-25.png" alt="decorative banner" width="1200"/>
</p>

# [Microsoft Ignite 2025](https://ignite.microsoft.com)

## 🔥PREL16: Preday: Implement Semantic Memories for Multi-Agent Apps in AI Foundry with an MCP Server for Azure Cosmos DB

### Session Description

Learn how to build intelligent, multi-agent apps with persistent, semantic memory using an MCP Server on Azure Cosmos DB. This hands-on workshop goes beyond basic memory storage to explore novel patterns for embedding and retrieving context across threads. Using LangGraph (Python) and Azure AI Foundry you’ll implement durable memory, semantic search, and agent collaboration. Leave with a scalable system that learns and adapts over time.

### 🧠 Learning Outcomes

# Learning Outcomes

By the end of this session, learners will be able to:

1. **Design and Implement Multi-Agent Systems**
Build sophisticated multi-agent architectures using LangGraph, including orchestrator patterns, agent specialization, and coordinated workflows between multiple AI agents with distinct roles and responsibilities.

2. **Master Agent-to-Agent Communication**
Configure seamless handoffs between specialized agents (Hotel, Dining, Activity, Itinerary Generator) using transfer mechanisms and state management to create cohesive user experiences across domain boundaries.

3. **Implement Production-Ready Agentic Memory Systems**
Design and deploy persistent memory architectures using Azure Cosmos DB, including declarative (facts), procedural (preferences), and episodic (experiences) memory types with salience scoring and TTL policies.

4. **Build Intelligent Preference Management**
Create LLM-powered systems that automatically extract user preferences from natural language, detect contradictory preferences, resolve conflicts, and maintain coherent user profiles across sessions.

5. **Configure Vector Search and Hybrid Retrieval**
Integrate Azure Cosmos DB vector search with embedding generation and hybrid search patterns (vector + BM25) to enable semantic discovery of hotels, restaurants, and activities based on user preferences.

6. **Implement Automatic Conversation Summarization**
Build background summarization systems that compress long conversations while preserving context, using span-based compression and intelligent memory consolidation to maintain conversation continuity.

7. **Deploy Observable Multi-Agent Systems**
Integrate comprehensive observability using LangSmith tracing to monitor agent interactions, debug complex workflows, track token usage, and visualize execution paths across distributed agent networks.

8. **Architect Tool Distribution Strategies**
Design Model Control Protocol (MCP) server architectures that strategically distribute tools across agents, manage external API integrations, and maintain consistent interfaces between agents and data sources.

9. **Handle Production Complexity**
Implement error handling, session management, conflict resolution, memory superseding, and state persistence patterns necessary for production multi-agent applications with real user interactions.

10. **Apply Agentic AI Best Practices**
Understand when to use multi-agent vs. single-agent patterns, how to balance automation with user control, manage computational costs, and design systems that gracefully handle edge cases and evolving requirements.

### 💻 Technologies Used

1. [Azure Cosmos DB](https://learn.microsoft.com/en-us/azure/cosmos-db/introduction)
   - [Vector Search](https://learn.microsoft.com/en-us/azure/cosmos-db/nosql/vector-search)
   - [Full Text Search](https://learn.microsoft.com/en-us/azure/cosmos-db/gen-ai/full-text-search)
   - [Hybrid Search](https://learn.microsoft.com/en-us/azure/cosmos-db/gen-ai/hybrid-search)
   - [Agentic Memory](https://learn.microsoft.com/en-us/azure/cosmos-db/gen-ai/agentic-memories)
2. [Azure OpenAI Service](https://learn.microsoft.com/azure/cognitive-services/openai/)
3. [Azure AI Foundry](https://learn.microsoft.com/en-us/azure/ai-foundry/)
4. [Langraph](https://www.langchain.com/langgraph)
5. [langSmith](https://docs.langchain.com/langsmith/home)

### 🚀 Getting Started

During Microsoft Ignite, this workshop is hosted in a virtual environment preconfigured with all necessary prerequisites and accounts.
If you’re running the workshop outside of Ignite, you can either follow the exercises step by step or use the provided completed files to launch the multi-agent travel assistant application directly.

#### Exercises:

Work through the exercises to build the application step by step:

- [LangGraph (Python)](https://github.com/AzureCosmosDB/travel-multi-agent-workshop/blob/main/01_exercises/workshop/Home.md)

#### Completed Files

If you prefer to skip the exercises and run as demo directly:

- [LangGraph (Python)](https://github.com/AzureCosmosDB/travel-multi-agent-workshop/blob/main/README.md)

## Content Owners

<table>
<tr>
    <td align="center"><a href="https://github.com/aayush3011">
        <img src="https://github.com/aayush3011.png" width="100px;" alt="Tiago Pascoal" "/><br />
        <sub><b> Aayush Kataria
</b></sub></a><br />
            <a href="https://github.com/aayush3011" title="talk">📢</a> 
    </td>
    <td align="center"><a href="https://github.com/TheovanKraay">
        <img src="https://github.com/TheovanKraay.png" width="100px;" alt="April Yoho"/><br />
        <sub><b>Theo van Kraay
</b></sub></a><br />
            <a href="https://github.com/TheovanKraay" title="talk">📢</a> 
    </td>
</tr></table>

## Resources & Next Steps

| Resource               | Link                                                                                                 | Description                                 |
|------------------------|------------------------------------------------------------------------------------------------------|---------------------------------------------|
| Ignite 2025 Next Steps | [https://aka.ms/Ignite25-Next-Steps](https://aka.ms/Ignite25-Next-Steps?ocid=ignite25_nextsteps_cnl) | Links to all repos for Ignite 2025 Sessions |

## Contributing

This project welcomes contributions and suggestions. Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit [Contributor License Agreements](https://cla.opensource.microsoft.com).

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft
trademarks or logos is subject to and must follow
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
