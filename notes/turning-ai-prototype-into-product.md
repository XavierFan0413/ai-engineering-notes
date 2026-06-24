# Turning an AI Prototype Into a Deployable Product

This note is a work-in-progress reflection on the engineering work required to move an AI prototype closer to a usable product.

## 1. A prototype is not the same as a product

An AI prototype can answer questions in a demo, but a deployable product needs more than model calls. It needs authentication, deployment, logging, testing, error handling, recovery flows, cost awareness, and clear user boundaries.

## 2. RAG needs operational discipline

Retrieval-augmented generation is not only about embedding documents and calling an LLM. The source documents need to be selected, updated, indexed, and verified. Retrieved context should also be treated as reference material, not as trusted instructions.

## 3. Guardrails need to handle real user behaviour

Users may ask unsafe, confused, incomplete, or adversarial questions. A useful system should refuse harmful requests without getting stuck in refusal mode for normal follow-up questions.

## 4. Cloud deployment creates practical issues

Once an application is live, issues become operational: CI/CD, task definitions, logs, environment variables, DNS, authentication, and email delivery all matter.

## 5. Governance evidence is engineering evidence

AI governance is not only policy writing. It depends on concrete evidence: architecture, model inventory, data handling, logs, guardrails, testing, human oversight, and known limitations.

## Notes to expand later

- RAG source document management
- Prompt injection and retrieved-context framing
- Authentication and email confirmation flows
- AWS deployment and rollback habits
- AI governance evidence checklists
