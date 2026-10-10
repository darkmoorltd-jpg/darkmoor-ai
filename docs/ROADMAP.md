# Darkmoor AI — 12 Month Roadmap

## Q4 2026 — GAIA Voice v1
- [ ] Download Google FLEURS (Yoruba, Igbo, Hausa)
- [ ] Augment with Common Voice
- [ ] Record 30 min × 9 speakers (3 languages × 3 speakers)
- [ ] Fine-tune XTTS-v2 (Yoruba, Igbo, Hausa)
- [ ] Deploy to Replicate
- [ ] Swap GAIA mobile /tts endpoint to GAIA Voice
- [ ] Cancel YarnGPT subscription

**Success metric:** 60%+ native accent match on blind listening test vs YarnGPT.

## Q1 2027 — GAIA Whisper
- [ ] Collect 500K mixed-language voice queries from GAIA usage
- [ ] Fine-tune Whisper-large-v3 on Nigerian accented English + Pidgin
- [ ] Deploy as /stt v2 endpoint
- [ ] A/B test against Groq Whisper

**Success metric:** 25%+ WER reduction on Pidgin audio.

## Q2 2027 — GAIA Brain v1
- [ ] Ship LLM training-data logging on all GAIA backends
- [ ] Accumulate 100K+ farm Q&A pairs
- [ ] Fine-tune Llama-3.2-3B (LoRA)
- [ ] Deploy as /chat_v2
- [ ] A/B test against Groq/DeepSeek

**Success metric:** 20%+ farmer-preference win rate vs GPT-4 on farm questions.

## Q3 2027 — GAIA Vision v2
- [ ] Ship vision-training-data logging on all GAIA diagnosis endpoints
- [ ] Accumulate 100K+ labeled Nigerian crop images
- [ ] Fine-tune ViT-Small on Nigerian-specific classes
- [ ] Quantize to INT8, deploy on-device
- [ ] Ship as `models/vision/gaia-maize-v2.onnx`

**Success metric:** 15%+ accuracy improvement on Nigerian test set.

## Q4 2027 — Public API
- [ ] Expose /voice, /brain, /vision as paid endpoints
- [ ] Stripe/Paystack billing
- [ ] SDK (Python, JS)
- [ ] First 5 external customers

**Success metric:** $10K MRR from model APIs alone.
