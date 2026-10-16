# Huddle demo: brief

_Updated 2026-10-16T18:15:16.526+00:00 by Huddle._

**Goal:** Research voice agents and AI tools for clinical backend operations—understand the landscape, demonstrate hands-on ElevenLabs prototype for key use cases with real API integration, and validate findings against real admin workflows with rigorous methodology and evidence tracing.

Prototype v2 is complete with real ElevenLabs API integration; live voice validation must use synthetic patients until Enterprise BAA is signed (ZRM removes transcripts/logs, requiring client-side accuracy logging). Assort Health is the main incumbent in scheduling/cancellation/confirmations; EHR integration, not voice alone, is the hard part. The team should prioritize intake and EHR write-back over the three commoditized use cases (scheduling, rescheduling, cancellation) to differentiate. Pipelines #2, #3, #5 remain in review pending revision for citation discipline, evidence mapping, and synthesis methodology. Scope decision must lock to unblock research finalization and prototype expansion.

## Decisions
_None yet._

## Open questions
- What are the main AI agent frameworks (e.g., LangChain, AutoGPT, CrewAI, others) and how do they compare for healthcare workflows?
- What clinical-specific tools and platforms already exist for admin workflow automation?
- What compliance/privacy considerations (HIPAA, etc.) are critical for clinical agent deployment?
- Should the prototype focus on the three commoditized use cases (scheduling, rescheduling, cancellation) where Assort Health competes, or pivot to patient intake + EHR write-back for differentiation?

## Ideas
- Focus research on real admin pain points (scheduling, documentation, triage) to inform which tools matter most
- Use ElevenLabs to prototype and demonstrate voice agent workflows for clinical operations (patient intake, scheduling, inquiries, follow-ups, rescheduling, cancellation)—core logic now validated in typed mode; v2 ready for live voice testing
- Prioritize patient intake and EHR write-back as the differentiation vector; scheduling/rescheduling/cancellation are commoditized and dominated by Assort Health (89% wait reduction, 57% less abandonment, 63% lower cost with 84+ EHR integrations)

## Next steps
- Decide: focus on intake + EHR write-back (defensible) or pursue the three commoditized use cases (schedule, reschedule, cancel)? This unlocks scope for research finalization and prototype expansion. (team)
- Build real integrated prototype for patient intake voice agent (build team)
- Run live voice validation of prototype v2: test end-to-end workflows with synthetic patients (no real PHI until Enterprise BAA is signed); ElevenLabs ZRM removes transcripts/logs, so implement client-side accuracy and performance logging. (build team)
- Revise pipelines #2, #3, #5: document search strategy (keywords, sources, inclusion criteria), synthesis methodology, vendor capability assessment; map each finding explicitly to prototype design decisions with direct evidence citations (research team)
