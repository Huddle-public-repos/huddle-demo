# Huddle demo: brief

_Updated 2026-10-16T18:42:59.135+00:00 by Huddle._

**Goal:** Research voice agents and AI tools for clinical backend operations—understand the landscape, demonstrate hands-on ElevenLabs prototype for key use cases with real API integration, and validate findings against real admin workflows with rigorous methodology and evidence tracing.

Prototype v2 with real ElevenLabs API integration was verified (#97), and the team decided to build and deploy a real integrated patient intake voice agent (#98). Pipeline #8 was tasked to build and deploy this; however, smoke testing (#108) revealed a critical API validation error (ElevenLabs requires turbo or flash v2 for English agents) and zero FHIR output from the mock EHR endpoint. The team is now repairing the app based on browser and server logs (#110) and will test again.

## Decisions
_None yet._

## Open questions
- What are the main AI agent frameworks (e.g., LangChain, AutoGPT, CrewAI, others) and how do they compare for healthcare workflows?
- What clinical-specific tools and platforms already exist for admin workflow automation?
- What compliance/privacy considerations (HIPAA, etc.) are critical for clinical agent deployment?
- Is the ElevenLabs agent configured with the correct model (turbo or flash v2), and why is the mock EHR endpoint returning zero results?

## Ideas
- Focus research on real admin pain points (scheduling, documentation, triage) to inform which tools matter most
- Build and deploy real patient intake voice agent on ElevenLabs Agents: Node server, intake system prompt (name, DOB, phone, reason, insurance, slot selection, confirmation), mock EHR FHIR output, typed mode for testing, synthetic patients only until Enterprise BAA signed
- Prioritize patient intake and EHR write-back as the differentiation vector; scheduling/rescheduling/cancellation are commoditized and dominated by Assort Health (89% wait reduction, 57% less abandonment, 63% lower cost with 84+ EHR integrations)

## Next steps
- Fix and retry smoke test for Pipeline #8: (1) verify ElevenLabs agent uses turbo or flash v2 model, (2) check mock EHR endpoint for data initialization and FHIR output, (3) test typed session connection, (4) run full intake conversation flow
