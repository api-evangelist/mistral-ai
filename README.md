# Mistral AI (mistral-ai)

Mistral AI is a French artificial intelligence company that develops and provides frontier large language models and APIs for developers and enterprises. Their developer platform offers APIs for chat completions, embeddings, fine-tuning, OCR, batch processing, and agentic workflows, enabling teams to build sophisticated AI-powered applications.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Agents
- Artificial Intelligence
- Batch Processing
- Chat
- Embeddings
- Fine-Tuning
- Large Language Models
- OCR

## Timestamps

- **Created:** 2025-03-07
- **Modified:** 2026-05-19

## APIs

### Mistral AI Chat Completions API

The Mistral AI Chat Completions API enables developers to interact with Mistral's language models in a conversational manner. It supports multi-turn conversations, function calling, and JSON mode for structured outputs. The API provides access to a range of models including Mistral Large, Mistral Small, and Codestral, each optimized for different use cases from general reasoning to code generation.

- **Human URL:** [https://docs.mistral.ai/api/endpoint/chat](https://docs.mistral.ai/api/endpoint/chat)
- **Base URL:** `https://api.mistral.ai/v1`

#### Tags

- Artificial Intelligence
- Chat
- Completions
- Conversational AI
- Large Language Models

#### Properties

- [Documentation](https://docs.mistral.ai/api/endpoint/chat)
- [OpenAPI](openapi/mistral-ai-chat-completions-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mistral-ai-chat-completions.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mistral-ai-chat-completions.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mistral AI Embeddings API

The Mistral AI Embeddings API allows developers to compute document and text embeddings using Mistral's embedding models. These embeddings can be used for semantic search, clustering, classification, and retrieval augmented generation workflows. The API accepts text inputs and returns high-dimensional vector representations suitable for a variety of natural language processing tasks.

- **Human URL:** [https://docs.mistral.ai/capabilities/embeddings](https://docs.mistral.ai/capabilities/embeddings)
- **Base URL:** `https://api.mistral.ai/v1`

#### Tags

- Artificial Intelligence
- Embeddings
- Semantic Search
- Vector Search

#### Properties

- [Documentation](https://docs.mistral.ai/capabilities/embeddings)
- [OpenAPI](openapi/mistral-ai-embeddings-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mistral-ai-embeddings.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mistral-ai-embeddings.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mistral AI Agents API

The Mistral AI Agents API provides a dedicated framework for building agentic applications. It complements the Chat Completion API by enabling AI agents to handle complex tasks, maintain context across interactions, and coordinate multiple actions. Developers can create agents with specific configurations, tools, and instructions, making it suitable for enterprise-grade agentic platforms and multi-step workflow automation.

- **Human URL:** [https://docs.mistral.ai/api/endpoint/agents](https://docs.mistral.ai/api/endpoint/agents)
- **Base URL:** `https://api.mistral.ai/v1`

#### Tags

- Agentic Workflows
- Agents
- Artificial Intelligence
- Automation
- Orchestration

#### Properties

- [Documentation](https://docs.mistral.ai/api/endpoint/agents)
- [OpenAPI](openapi/mistral-ai-agents-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mistral-ai-agents.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mistral-ai-agents.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mistral AI Fine-Tuning API

The Mistral AI Fine-Tuning API allows developers to create and manage fine-tuning jobs that customize Mistral models on proprietary datasets. Users can upload training data, configure hyperparameters, and monitor job progress through the API. Fine-tuned models can then be deployed and accessed through the Chat Completions endpoint, enabling domain-specific performance improvements for enterprise applications.

- **Human URL:** [https://docs.mistral.ai/api/endpoint/fine-tuning](https://docs.mistral.ai/api/endpoint/fine-tuning)
- **Base URL:** `https://api.mistral.ai/v1`

#### Tags

- Artificial Intelligence
- Customization
- Fine-Tuning
- Machine Learning
- Model Training

#### Properties

- [Documentation](https://docs.mistral.ai/api/endpoint/fine-tuning)
- [OpenAPI](openapi/mistral-ai-fine-tuning-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mistral-ai-fine-tuning.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mistral-ai-fine-tuning.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mistral AI OCR API

The Mistral AI OCR API provides optical character recognition capabilities powered by the mistral-ocr-latest model. It can extract text and structured content from PDF documents and images, comprehending complex document elements including media, tables, equations, and interleaved text. The API returns ordered, structured content suitable for downstream processing and retrieval augmented generation pipelines.

- **Human URL:** [https://docs.mistral.ai/api/endpoint/ocr](https://docs.mistral.ai/api/endpoint/ocr)
- **Base URL:** `https://api.mistral.ai/v1`

#### Tags

- Artificial Intelligence
- Document AI
- OCR
- PDF Processing
- Text Extraction

#### Properties

- [Documentation](https://docs.mistral.ai/api/endpoint/ocr)
- [OpenAPI](openapi/mistral-ai-ocr-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mistral-ai-ocr.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mistral-ai-ocr.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mistral AI Models API

The Mistral AI Models API provides endpoints for listing and retrieving information about available models on the Mistral platform. Developers can query which models are accessible, inspect model capabilities and metadata, and manage fine-tuned model deployments. This API serves as the foundation for model discovery and lifecycle management within the Mistral ecosystem.

- **Human URL:** [https://docs.mistral.ai/api/endpoint/models](https://docs.mistral.ai/api/endpoint/models)
- **Base URL:** `https://api.mistral.ai/v1`

#### Tags

- Artificial Intelligence
- Infrastructure
- Model Management
- Models

#### Properties

- [Documentation](https://docs.mistral.ai/api/endpoint/models)
- [OpenAPI](openapi/mistral-ai-models-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mistral-ai-models.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mistral-ai-models.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mistral AI Forge API

Mistral AI Forge is a model-training platform providing a unified API for the entire model lifecycle from pre-training to reinforcement learning. Forge enables enterprises to build frontier-grade AI models grounded in proprietary knowledge, supporting pre-training on large internal datasets, post-training through supervised fine-tuning with DPO and ODPO, and reinforcement learning pipelines for aligning models with internal policies. Forge is optimized for agentic workflows, allowing AI agents to programmatically schedule training jobs, optimize hyperparameters, and generate synthetic data. The platform supports both Dense and Mixture-of-Experts model architectures with serverless infrastructure.

- **Human URL:** [https://mistral.ai/news/forge](https://mistral.ai/news/forge)

#### Tags

- Agentic Workflows
- Artificial Intelligence
- Enterprise AI
- Model Training
- Pre-Training
- Reinforcement Learning

#### Properties

- [Documentation](https://mistral.ai/news/forge)
- [OpenAPI](openapi/mistral-ai-forge-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mistral-ai-forge.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mistral-ai-forge.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mistral AI Batch API

The Mistral AI Batch API enables developers to submit large volumes of requests for asynchronous processing at reduced cost. It is designed for workloads that do not require real-time responses, such as bulk text classification, large-scale content generation, and data processing pipelines. Developers can submit batch jobs, monitor their progress, and retrieve results once processing is complete.

- **Human URL:** [https://docs.mistral.ai/capabilities/batch](https://docs.mistral.ai/capabilities/batch)
- **Base URL:** `https://api.mistral.ai/v1`

#### Tags

- Artificial Intelligence
- Asynchronous
- Batch Processing
- Large Scale

#### Properties

- [Documentation](https://docs.mistral.ai/capabilities/batch)
- [OpenAPI](openapi/mistral-ai-batch-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mistral-ai-batch.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mistral-ai-batch.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/mistralai)
- [LinkedIn](https://www.linkedin.com/company/mistralai)
- [Portal](https://console.mistral.ai/)
- [Documentation](https://docs.mistral.ai/)
- [Website](https://mistral.ai/)
- [Privacy Policy](https://mistral.ai/terms/#privacy-policy)
- [Terms of Service](https://mistral.ai/terms/#terms-of-use)
- [Blog](https://mistral.ai/news/)
- [Login](https://console.mistral.ai/)
- [JSON-LD](json-ld/mistral-ai-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/mistral-ai-chat-completion-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/mistral-ai-model-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/mistral-ai-fine-tuning-job-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/mistral-ai-batch-job-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/mistral-ai-ocr-response-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Integrations](https://mistral.ai/partners)
- [L L Ms Txt](https://docs.mistral.ai/llms.txt)

## Maintainers

**FN:** API Evangelist
**Email:** info@apievangelist.com
