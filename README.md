# ORION

**Local AI studio — thinking companion, media generation, lip-sync.**

ORION is a desktop AI application that runs entirely on your machine.
No cloud, no subscriptions, no data leaving your computer.

---

## Download

**macOS (Apple Silicon — M1/M2/M3/M4):**

1. Download `ORION.dmg` from [Releases](../../releases)
2. Open the `.dmg` file
3. Drag **ORION** into **Applications**
4. Launch ORION from Launchpad or Applications folder

> **Requirements:** macOS 12.0+, Apple Silicon (M1+), 16 GB RAM minimum (32 GB recommended)

---

## First Launch

ORION's setup wizard will guide you through:

1. **Ollama** (LLM engine) — install with one click from the wizard
2. **ffmpeg** (video processing) — install via Homebrew from the wizard
3. **AI Models** — download core models (~5 GB) with one click

The wizard checks your system and shows what's ready and what needs installing.

---

## Features

### NEXUS — AI Dialogue
- Natural conversation with local LLM (Qwen, Llama, etc.)
- Self-awareness: identity, memory, self-tuning
- Web search integration
- Semantic + episodic memory
- Multi-agent reasoning (optimist, pessimist, realist, disruptor)
- Scenario radar with risk/impact/confidence visualization

### ATELIER — Cinematic Pipeline
- Idea → Script → Storyboard → Render → Animation → Final MP4
- One-click full auto-run
- Style presets: photoreal, anime, cyberpunk, cartoon
- Powered by ComfyUI (SDXL, LTX-Video)

### FORGE — Code Workshop
- Streaming code generation with syntax highlighting
- Slash commands: /review, /refactor, /explain, /test, /generate, /fix, /run
- Safe sandbox execution
- Multi-file generation
- Project scanner + snippet library
- One-click `.command` launcher for generated code

### Media Generation
- Image generation via ComfyUI (SDXL)
- Video generation via LTX-Video
- LatentSync — lip-sync for talking-head videos
- LivePortrait — facial animation from a single photo

### Voice
- Real-time speech-to-text + text-to-speech loop
- Multiple TTS engines: macOS `say`, Chatterbox, Qwen3-TTS

---

## Licensing

ORION comes with a **7-day full-access trial**.

After the trial:
- **Free:** NEXUS dialogue, basic features
- **Pro:** ATELIER pipeline, FORGE, media generation, LatentSync, LivePortrait

To activate Pro:
1. Purchase a license key
2. Open ORION → Menu bar → License → Activate
3. Enter your email and key

---

## Optional Backends

These are detected automatically. The setup wizard provides install instructions.

### ComfyUI (image/video generation)
- Install [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
- Place checkpoints in `ComfyUI/models/checkpoints/`
- Recommended: `DreamShaperXL_Lightning.safetensors`, `ltx-video-2.3.safetensors`

### LatentSync (lip-sync)
- Clone [LatentSync](https://github.com/bytedance/LatentSync) to `~/latentsync`
- Follow their setup instructions
- Download model checkpoints

### LivePortrait (facial animation)
- Clone [LivePortrait](https://github.com/KwaiVGI/LivePortrait)
- Follow their setup instructions

---

## Core Models

ORION uses these Ollama models (auto-downloaded by the setup wizard):

| Model | Purpose | Size |
|-------|---------|------|
| `qwen2.5:7b-instruct-q4_K_M` | Conversation + analysis | ~4.7 GB |
| `bge-m3` | Embeddings for memory | ~1.2 GB |

For systems with 32 GB+ RAM, `qwen2.5:32b-instruct-q4_K_M` is recommended for better dialogue quality.

---

## Privacy

- **All processing is local.** No data sent to any server.
- Conversations, memory, and settings stored in `~/Documents/ORION/`
- Web search (optional) goes through DuckDuckGo
- No telemetry, no analytics, no tracking

---

## Support

- **Issues:** [GitHub Issues](../../issues)
- **Email:** support@matoka.studio

---

## Credits

**ORION** — built by [MATOKA](https://matoka.studio)

Powered by: Ollama, PyTorch, PySide6, ComfyUI, LatentSync, LivePortrait, transformers
