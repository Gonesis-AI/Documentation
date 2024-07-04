# Workflow

## Introduction

Workflow defines what an AI agent can do. It simplifies the development of AI agents by breaking down complex tasks into smaller, manageable steps (nodes). This method reduces reliance on prompt engineering and model inference skills, thereby increasing the efficiency of LLM applications for intricate tasks. Moreover, it enhances system clarity, robustness, and fault tolerance.

## Key Concepts

### 1. Nodes

**Nodes are the key components of a workflow**. enabling the execution of a series of operations by connecting nodes with different functionalities.

### 2. Variables

**Variables are used to link the input and output of nodes within a workflow**, enabling complex processing logic throughout the process.

* The output variables of nodes are system-fixed and cannot be edited.
* Node names must be unique to avoid conflicts.
* Only upstream node variables can be referenced in the process.
* Nodes typically define input variables, e.g., `sys.query` for a question classifier.
* Workflows need to specify execution start variables, like `sys.query` for a chatbot.

### 3. Edges

Edges must connect exactly **two** **Nodes** within the workflow. Edges indicate the flow from the source node to the target node, establishing the order of operations.

## Supported Workflow

As an open protocol, our goal is not to create a new workflow data structure. Instead, we aim to create a unified platform that ensures maximum compatibility with existing workflow structures available on the market.

We will support the following workflow formats(only open-source):

<table><thead><tr><th width="166">Platform</th><th width="173">Engine Name</th><th>Documentation</th></tr></thead><tbody><tr><td>ComfyUI</td><td><code>comfy</code></td><td><a href="https://github.com/comfyanonymous/ComfyUI">https://github.com/comfyanonymous/ComfyUI</a></td></tr><tr><td>Dify.ai</td><td><code>dify</code></td><td><a href="https://docs.dify.ai/guides/workflow">https://docs.dify.ai/guides/workflow</a></td></tr><tr><td>LangGraph</td><td><code>langgraph</code></td><td><a href="https://langchain-ai.github.io/langgraph/">https://langchain-ai.github.io/langgraph/</a></td></tr><tr><td>Crewai.com</td><td><code>crewai</code></td><td><a href="https://docs.crewai.com/">https://docs.crewai.com/</a></td></tr><tr><td>AutoGen Studio</td><td><code>autogen</code></td><td><a href="https://microsoft.github.io/autogen/docs/Getting-Started">https://microsoft.github.io/autogen/docs/Getting-Started</a></td></tr><tr><td>Langflow.org</td><td><code>langflow</code></td><td><a href="https://docs.langflow.org/">https://docs.langflow.org/</a></td></tr><tr><td>Fastgpt.in</td><td><code>fastgpt</code></td><td><a href="https://doc.fastgpt.in/docs/">https://doc.fastgpt.in/docs/</a></td></tr></tbody></table>

You can also use open-source tools like LangChain to create custom workflow formats and integrate them into the AI721 protocol.

## How to Run Workflows

Neuro Node runners use the engine service to provide unified API gateways and execute workflows on demand. You can also run a local node service to test the process.

Neuro Nodes can flexibly choose to call LLMs through the `llm` field API, use specific LLM APIs defined in the workflow nodes, or opt for lower-cost custom local LLMs. Gonesis provides this flexibility to adapt to various scenarios.
