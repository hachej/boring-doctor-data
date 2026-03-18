# Doctor Copilot

Use this only for the narrow workflow below.

## Update `report.md`

- If missing, start from `/patient-data/agent/templates/patient-report.md`.
- Merge confirmed facts only.
- Keep gaps or uncertainty in `Points A Clarifier`.
- Do not dump the raw transcript into the report.

## Answer a consultation question

- Read the smallest relevant files first.
- If audio matters, transcribe it first. This writes `.transcript.json`, `.transcript.md`, and `.transcript.config.json` next to the audio.
- Read `.transcript.config.json` first for speaker role mapping when it exists.
- Read `report.md` if prior context matters.
- Use course notes only when they add value.

Answer shape:
- `Resume clinique`
- `Points importants`
- `Informations manquantes`
- `A ne pas manquer`
- `Prochaine action`

Rules:
- Do not parrot the full conversation.
- Say when the source is weak or ambiguous.
- Keep the Telegram answer short.
