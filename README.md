# Claude Mogger

A local-first, multi-model AI chat workspace built with vanilla HTML/CSS/JavaScript and Puter.js.

## Current MVP

- Live model catalogue using `puter.ai.listModels()`
- Model search and selection
- Streaming chat using `puter.ai.chat()`
- Browser-local conversation history
- JSON workspace export/import and Markdown import
- Optional Puter sign-in and KV sync
- Responsive layout

## Run

Open `index.html` in a modern browser, or serve this folder with any static web server. Puter.js is loaded from its official CDN and requires an internet connection.

## Data and privacy

Conversation history is stored in this browser's localStorage. Cloud sync is opt-in and stores the app workspace in the signed-in user's Puter KV namespace. Cloud sync is not a substitute for local exports. API keys are not requested or stored by this MVP.

## Roadmap

- Provider adapters and BYOK through a localhost companion service (planned default port: 6767)
- OpenAI-compatible local API gateway with app-issued keys
- MCP server/client integration and plugin management
- Native importers for ChatGPT, Claude, Gemini and other export archives
- Safer sync conflict resolution, backup versioning, and attachment support
- More free-provider integrations where officially supported

Provider availability, usage limits, quotas, and pricing are controlled by the relevant provider. This app does not bypass those controls.
