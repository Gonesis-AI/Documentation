---
description: >-
  A knowledge base service with low barriers, high scalability, and privacy
  protection, built for AI agents.
---

# G-KB (Gonesis Knowledge Base)

## What is Knowledge Base

A knowledge base is a collection of information(documents, texts, structured data) that can be integrated into an application as a retrieval context. The information can be uploaded by creators of AI agents, or synchronized from other data sources.

## Why We Need Knowledge Base

Training large language models relies on public data and requires significant computational power. As a result, they typically lack private domain knowledge and may be behind on the latest public information.

To address this problem, the common solution is to use [Retrieval-Augmented Generation (RAG)](retrieval-augmented-generation-rag.md). This technology matches user queries with the most relevant external data, retrieves the content, and integrates it into the model prompt to generate a response.

## Introducing G-KB (Gonesis Knowledge Base)

Currently, centralized AI agent platforms require users to upload their private knowledge to a centralized database. **It easily leads to plagiarism and privacy breaches.** Furthermore, it obstructs the growth of a wider AI agent ecosystem.

To address this issue, we introduce **G-KB(Gonesis Knowledge Base). It can be run as a standalone storage service, or integrated seamlessly as an extension module within** [**Agent Creator Platforms**](../ai-creator-platform.md)**.**

**G-KB** allows creators to securely upload their private knowledge to an access-controlled database, and connect it with AI agent workflows, while protecting the confidentiality of their knowledge bases. It also ensures high reliability, fast response times and unlimitied scalability.

### Features and Advantages

1. **Supports Local and Decentralized Storage**: G-KB can store data in the local or decentralized storage networks(like arweave or filecoin), providing flexibility and robustness.
2. **Privacy and Access Control**: Ensures data privacy and secure access using advanced cryptographic methods.
3. **Extensibility and Composability**: Allows linking to external data sources or other knowledge bases via embedded URLs, saving storage space.
4. **Out-of-the-box UI**: Provides a simple and easy-to-use user interface for uploading and managing knowledge bases.
5. **API-based External Access**: Provides seamless integration and access for external AI agents and applications via customizable APIs.
6. **Open-source**: Fully open-source, enabling customization and further development as needed.

## Repository

The codes of G-KB will be totally open-source. The repo is coming soon.
