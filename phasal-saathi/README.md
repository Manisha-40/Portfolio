# Phasal Saathi — AI-enabled agricultural coordination concept

**One message. The right help. No office runaround.**

Phasal Saathi is a WhatsApp-first proposed coordination layer between farmers, Farmer Producer Organizations (FPOs), Krishi Vigyan Kendras (KVKs), and the Agriculture Department, grounded in fieldwork in Sikkim.

## Open the prototype

Open `index.html` in a modern browser. It is a self-contained, interactive HTML demonstration; no package installation or API key is needed.

## Try the AI Trace

1. Select **Sell produce**, **Crop concern**, or **Scheme help**.
2. Choose the WhatsApp-style channel or optional mobile app and a language preview.
3. Select **✨ AI trace** on the right to inspect every stage.
4. On the phone, edit the sample farmer message; enter *80 kg ginger* to see the structured fields and market arithmetic change.
5. Inspect mocked retrieval records and missing data, deterministic decision policy, expert escalation, and business-outcome measures.
6. In **Failure tests**, test offline WhatsApp and an unclear transcription.

## Where AI fits (proposed, not deployed)

| Stage | Proposed capability | Authority / safety |
| --- | --- | --- |
| Intake | ASR and multilingual language interpretation | Confirm transcription with farmer |
| Understanding | LLM extracts intent, crop, location, quantity and missing fields | Clarify ambiguity |
| Retrieval | RAG over approved KVK references, current FPO quotes and official scheme rules | Date and cite every source; abstain if absent |
| Decision | Ordinary rules for eligibility checks and financial calculations | Do not let an LLM improvise rules or prices |
| Explanation | LLM simplifies verified results in supported languages | Show uncertainty and verification status |
| Coordination | Routed tasks and follow-up tracking | KVK validates agronomy; officials confirm eligibility; FPO validates quotes |

**Important:** This demo does NOT call Gemini, speech-to-text, image recognition, a vector database, WhatsApp, government systems, or institutional messaging endpoints. It uses sample transcripts, deterministic extraction, mock sources and simulated case statuses. An attached crop image is a local preview, **not** a diagnosis. Never use the sample guidance or prices for real farming decisions.

## Business hypothesis & pilot

A ~350-farmer pilot was proposed; no live users or economic improvements are claimed here. Pilot outcomes would include farmer understanding, accurate eligibility responses, time to specialist closure, source-grounding errors, verified buyer outcomes, and farmer net receipts. The comparison of FPO and direct trade uses synthetic prices and transport costs to demonstrate rule-based calculation; current quotations require human verification.

## Deployment

Static HTML. In Vercel, import `Manisha-40/Portfolio`, choose **Other** framework, and set Root Directory to `phasal-saathi`. No build command, secret or database is needed. **Updating GitHub does not establish that Vercel has deployed**; check the Vercel project to confirm the latest production deployment.
