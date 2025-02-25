# Multi-agent Self-Reflective RAG with LangGraph Workshop

This repository offers resources and instructions for a hands-on workshop centered on utilizing LangGraph to develop and orchestrate multiple agents, each equipped with specific tools to accomplish tasks. The workshop guides participants through building a basic agentic application employing the Self-Reflective Retrieval-Augmented Generation (Self-RAG) pattern, as outlined by LangChain. ([blog.langchain.dev](https://blog.langchain.dev/agentic-rag-with-langgraph/?utm_source=chatgpt.com))

## Prerequisites

Before starting, ensure you have the following:

- **Azure OpenAI Resource**: Have your endpoint URL and API key ready.
- **GPT-4o Model Deployed**: Deploy the latest GPT-4o model with standard deployment in your OpenAI resource. Note that you'll need the deployment name for later use.
- **VS Code**: Install Visual Studio Code.

## Executing the Agentic Application

### Overview

![diagram.png](diagram.png)

In this workshop, we develop a main agent that processes user queries related to Lilian Weng's work on Large Language Models (LLMs). The agent utilizes tools to retrieve relevant documents and mechanisms to refine user queries, enhancing the quality of responses based on available content. This approach demonstrates how modifying the agent's state history can improve response quality.

The **retrieve** tool accesses external content stored in a vector store, complete with metadata describing its capabilities. If necessary, the **rewrite** agent reformulates the user prompt to better align with the application's purpose and available content, facilitating more effective document retrieval.

### Running in Jupyter Notebook

1. Open the **self-reflective_rag.ipynb** file.
2. Hover over the top code block and click the *play* button that appears at the top-left corner of the block. This action will prompt you to enter your Azure OpenAI API key in a pop-up within VS Code. The notebook provides guidance on the function of each block and the implementation of the Self-Reflective RAG pattern using the LangGraph framework.

## Conclusion

By the end of this workshop, you will have gained hands-on experience in building and modifying flows within prompt flow. Additionally, you will have learned how to evaluate their performance using a testing dataset.

For a visual walkthrough of implementing Self-RAG with LangGraph, you might find the following video tutorial helpful:

[Adaptive RAG with Self-Reflection: Part-1](https://www.youtube.com/watch?v=8UZCmQ8hP9c&utm_source=chatgpt.com)