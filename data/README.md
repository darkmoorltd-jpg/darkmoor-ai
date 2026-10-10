# Data

## Voice data (training)

Sources:
- **Google FLEURS** — CC-BY 4.0
- **Mozilla Common Voice** — CC-0
- **Proprietary recordings** — Darkmoor AI owned

Audio files are NOT committed. Metadata CSVs are.

## Vision data (training)

Collected via GAIA app with consent:
- Crop scan images
- User-corrected labels
- Location (state-level only)
- Language

Stored in Supabase `gaia_vision_training` table.

## Brain data (training)

Collected via GAIA app with consent:
- Chat prompts and responses
- Voice transcripts
- Language, crop, state context
- Feedback signals

Stored in Supabase `gaia_llm_training` table.

## Privacy

All training data is anonymized before export. No phone numbers,
no exact GPS, no personal identifiers. Only behavioral + agronomic
signals.
