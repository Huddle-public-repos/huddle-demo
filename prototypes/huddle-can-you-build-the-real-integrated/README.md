# Huddle can you build the real integrated prototype for the patient intake voice agent for 

Single-screen Riverside Clinic scheduling intake agent, locked to intake → scheduling → confirmation (no scope selector). Paste your ElevenLabs API key, click "Verify key", then "Start call". The agent speaks via ElevenLabs TTS, and the mic uses ElevenLabs Scribe STT. Typed replies also work, and are the fallback if the sandbox blocks the mic. To try it, answer with "Maria Alvarez", "03/14/1986", "annual physical", "the second one", "yes". The schedule panel, tool-call log, and traceability table update as you go; the clinic backend and SMS are mocked, and the key stays in memory only.

**Evals:** none
