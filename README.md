# Repo Goal

- this repo is to learn about AI Agents frameworks together, apply the concepts we will learn and try different tools and technologies.

## Table of Contents

- [Chapter 1: Introduction to AI Agents](#chapter-1-introduction-to-ai-agents)
  - [When to Use Agent Frameworks](#when-to-use-agent-frameworks)
  - [Smolagents Library](#smolagents-library)
  - [Types of Agents in Smolagents](#types-of-agents-in-smolagents)
  - [Getting Started](#getting-started)

## Chapter 1: Introduction to AI Agents

### When to Use Agent Frameworks

Before diving into agent frameworks, it's important to consider whether you actually need this level of abstraction. Here are some key points to consider:

- If your use case is simple, plain Python code might be sufficient
- Consider using an agent framework when you need:
  - A complex agent powered by an LLM engine
  - A set of tools for the agent to interact with
  - A parser to handle LLM outputs for correct function/tool calling

### Smolagents Library

This is a lightweight library to build simple and efficient agents. We'll be using this framework to learn and implement various agent types.

#### Types of Agents in Smolagents

1. **CodeAgent**
   - Instead of generating JSON or text, it generates Python code that executes
   - This is the main type used in the Smolagents framework
   - It's a type of MultiStepAgent

2. **Toolcalling Agent**
   - Outputs in JSON or text format
   - Requires parsing of the output

3. **Retrieval Agents**
   - Provides model access to knowledge bases
   - Can work with both web and custom knowledge bases

### Getting Started

In the following sections, we'll build our first CodeAgent using the smolagents framework. This will help us understand the basic concepts and implementation details of AI agents.

### Project Setup

Our project uses the following key components:

1. **Smolagents Framework**
   - A lightweight library for building AI agents
   - [GitHub Repository](https://github.com/huggingface/smolagents)

2. **OpenTelemetry with Langfuse**
   - We've integrated OpenTelemetry with Langfuse for tracing our LLM agent
   - This helps us monitor and analyze the agent's performance
   - [Langfuse GitHub Repository](https://github.com/langfuse/langfuse)
   - Below is a screenshot from our Langfuse portal showing the agent's performance metrics:

   ![Langfuse Portal Screenshot](/smolagents/images/image.png)

3. **Project Structure**
   - `smolagents/` - Main implementation directory
   - `.env` - Environment variables for configuration
