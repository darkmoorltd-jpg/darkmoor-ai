# GAIA Voice

Native African text-to-speech.

## Base model

XTTS-v2 (Coqui, 470M params) — multilingual base, fine-tuned per language.

## Training data

| Source | Language | Hours | License |
|---|---|---|---|
| Google FLEURS | Yoruba | ~10 | CC-BY 4.0 |
| Google FLEURS | Igbo | ~6 | CC-BY 4.0 |
| Google FLEURS | Hausa | ~12 | CC-BY 4.0 |
| Mozilla Common Voice | Yoruba | ~10 | CC-0 |
| Mozilla Common Voice | Igbo | ~4 | CC-0 |
| Mozilla Common Voice | Hausa | ~15 | CC-0 |
| Proprietary recordings | All 3 | TBD | Owned |

Target: 40+ hours per language before first fine-tune.

## Compute

- Training: 1× A100 40GB, ~40 hours per language
- Cost: ~$80 per language on RunPod
- Inference: Replicate or RunPod Serverless

## Deployment

- Export to ONNX or TorchScript
- Serve via FastAPI
- Endpoint: `POST /tts { text, language }` → returns MP3
- Replaces YarnGPT at `/tts`

## Voice design

Each language gets one "GAIA default" voice, tuned for clarity at low bandwidth:
- Warm, unhurried
- Slight Nigerian cadence
- Clear consonants for phone-speaker playback
- Rate: ~0.92× normal pace

Optional: gender variants per language.
