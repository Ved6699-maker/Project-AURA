# Secure online AI backend — planned

This directory is documentation only; no AI provider is connected yet.

A backend is required for online AI because the provider API key must remain private. A production backend should:
- Store provider API keys in hosting environment variables, never source files.
- Validate request size and content and apply rate limits.
- Restrict CORS to the exact deployed frontend origin.
- Avoid logging private conversation content by default.
- Provide clear privacy disclosures before storing or transmitting chats.
- Return JSON like {"reply":"..."} from POST /api/chat.

The frontend can be configured with window.AURA_API_URL set to the backend base URL once a tested endpoint is deployed.
