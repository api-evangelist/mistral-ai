# Mistral AI GraphQL Schema

This directory contains a conceptual GraphQL schema for the Mistral AI API, derived from the official REST API documented at [https://docs.mistral.ai/api/](https://docs.mistral.ai/api/). Mistral AI does not currently publish a native GraphQL endpoint; this schema expresses the same capabilities and data structures in GraphQL terms to support tooling, federation, and schema-driven development workflows.

## Source

- API Reference: https://docs.mistral.ai/api/
- GitHub Organization: https://github.com/mistralai
- Base URL: https://api.mistral.ai/v1

## Schema File

`mistral-ai-schema.graphql`

## Coverage

The schema covers all major Mistral AI API surface areas:

### Models
- `Model` — a Mistral language model with capabilities, permissions, and status
- `ModelDetails` — technical metadata including context window and architecture
- `ModelCapabilities` — feature flags (chat, embedding, vision, fine-tuning, etc.)
- `ModelSize`, `ModelParameters`, `VocabSize` — size and parameter descriptors
- `ContextLength` — input/output token limits
- `ModelPermission` — access control entries per model
- `ModelPurpose`, `ModelStatus` — enumerations for model classification

### Chat Completions
- `ChatCompletion` — full response object
- `Choice` — a single generated completion candidate
- `ChatCompletionDelta`, `StreamEvent`, `StreamChoice` — streaming support
- `SystemMessage`, `UserMessage`, `AssistantMessage`, `ToolMessage` — message variants
- `ChatMessage` — union of all message types
- `FinishReason` — stop, length, tool_calls, content_filter, error

### Tokens and Logprobs
- `Usage`, `TokenUsage` — token consumption statistics
- `Logprob`, `LogprobContent`, `TopLogprob` — token-level log-probability data

### Embeddings
- `Embedding`, `EmbeddingResponse`, `EmbeddingData` — embedding response types
- `TextInput`, `Tokens`, `VectorData` — input and vector representations
- `EmbeddingEncoding` — float or base64 encoding options

### Fill-In-the-Middle (FIM / Code Completion)
- `FIMRequest`, `FIMCompletion`, `FIMChoice`, `FIMDelta` — code completion types

### Tools and Function Calling
- `Tool`, `Function`, `FunctionDefinition`, `FunctionParameters` — tool definitions
- `ToolCall`, `ToolCallResult`, `FunctionCall`, `ParsedArgs` — invocation and results
- `JSONSchema` — schema objects for structured output and tool parameters
- `ToolChoiceMode` — auto, none, any, required

### Safety and Moderation
- `SafetyFilter`, `SafeguardConfig`, `ContentPolicy` — safety configuration
- `ModerationResult`, `CategoryScore`, `Category`, `Severity` — moderation results

### Response Formats
- `ResponseFormat`, `ResponseFormatType` — text vs. JSON object modes
- `JSONResponse`, `TextResponse` — typed response wrappers

### API Management
- `APIKey`, `APIClient` — key management and client configuration
- `UsageStat`, `ModelUsageStat` — aggregated usage reporting
- `RateLimit` — rate limiting metadata

### Fine-Tuning
- `FineTuningJob`, `FineTuningHyperparameters` — job configuration and state
- `FineTuningEvent`, `FineTuningIntegration` — logging and external integrations
- `FineTuningJobStatus` — queued, started, running, failed, success, cancelled

### Batch Processing
- `BatchJob`, `BatchError` — asynchronous batch job lifecycle
- `BatchJobStatus` — queued, running, success, failed, timeout, cancelled

### OCR
- `OCRDocument`, `OCRResponse`, `OCRPage` — document and page extraction
- `OCRImage`, `OCRDimensions`, `OCRUsage` — image regions and page metadata
- `OCRDocumentType` — PDF or image input

### Agents
- `Agent`, `AgentConversation` — agent configuration and conversation threads
- `AgentStatus` — active, inactive, archived

## Type Count

The schema defines **67 named types** (object types, enums, unions, scalars, and input types).

## Operations

### Queries
- `models` / `model` — list and retrieve models
- `fineTuningJobs` / `fineTuningJob` — list and retrieve fine-tuning jobs
- `batchJobs` / `batchJob` — list and retrieve batch jobs
- `apiKeys` — list API keys
- `usageStats` — aggregate usage over a time range
- `agents` / `agent` — list and retrieve agents

### Mutations
- `createChatCompletion` — generate a chat completion
- `createEmbedding` — compute embeddings
- `createFIMCompletion` — fill-in-the-middle code completion
- `createOCR` — extract text from documents or images
- `createFineTuningJob` / `cancelFineTuningJob` — manage fine-tuning jobs
- `createBatchJob` / `cancelBatchJob` — manage batch jobs
- `createAPIKey` / `deleteAPIKey` — manage API keys
- `createAgent` / `updateAgent` / `deleteAgent` — manage agents

### Subscriptions
- `chatCompletionStream` — stream tokens from a chat completion
- `fimCompletionStream` — stream tokens from a FIM completion
- `fineTuningJobUpdates` — watch a fine-tuning job for status changes
- `batchJobUpdates` — watch a batch job for progress
