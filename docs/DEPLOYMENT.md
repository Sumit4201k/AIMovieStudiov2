# Deployment & Driver Configuration

## Local Development (Docker Compose)

1. Copy `.env.example` to `.env` inside `backend/` and fill in your provider keys (`FAL_KEY`, `REPLICATE_API_TOKEN`, or local ComfyUI endpoint).
2. Start the full stack:

```bash
docker compose up --build
```

- **Backend API:** `http://localhost:8000` (Swagger docs at `/docs`)
- **Frontend Studio:** `http://localhost:3000`

## Supported Inference Drivers

| Domain | Drivers |
| :--- | :--- |
| Image Generation | ComfyUI (local/remote), Fal.ai, Flux2 |
| Video Generation | ComfyUI LTX-Video 2.3, Fal.ai, Replicate, MiniMax |
| Audio & Foley | Chatterbox TTS, Fish Speech, Hunyuan Foley |
| Scene Continuity | Character sheet & turnaround workflow presets (`backend/core/workflows/`) |
