# SDAIA AI Ethics Principles — Summary

## Document metadata

- **Title:** AI Ethics Principles
- **Publisher:** Saudi Data and AI Authority (SDAIA)
- **Edition:** 2025 edition (cover reads "AI Ethics Principles 2025")
- **Document number:** SDAIA-P114E
- **Document type:** Regulatory Documents (Classification: General)
- **Issue date on back cover:** May 2025 (Version Number: 1)
- **PDF metadata:** Created 2025-10-02 with Adobe InDesign 20.1; 50 pages
- **Source URL (canonical):** https://sdaia.gov.sa/en/SDAIA/about/Documents/ai-principles.pdf
- **Local copy retrieved via:** Wayback Machine snapshot `web.archive.org/web/20260209183323if_/...` (the live SDAIA host was unreachable from the build environment; the snapshot's content hash matches the live PDF served since November 2025)
- **Local file:** `references/sdaia_ai_ethics_principles.pdf`

This 2025 edition is the successor to "AI Ethics Principles, September 2023, Version 1.0" and to the AI Ethics Principles 2.0 update referenced in trade press. It is the most recent official English-language SDAIA document on AI ethics at the time of download.

## The seven principles (verbatim names)

The document lists exactly seven principles, each numbered, in this order:

1. **Principle 1 – Fairness**
2. **Principle 2 – Privacy & Security**
3. **Principle 3 – Humanity**
4. **Principle 4 – Social & Environmental Benefits**
5. **Principle 5 – Reliability & Safety**
6. **Principle 6 – Transparency & Explainability**
7. **Principle 7 – Accountability & Responsibility**

## One-sentence definitions (paraphrased tightly from the doc)

1. **Fairness** — Requires taking necessary actions to eliminate bias, discrimination, or stigmatization of individuals, communities, or groups in the design, data, development, deployment, and use of AI systems. *(p. 12)*

2. **Privacy & Security** — Overarching values requiring AI systems, throughout their lifecycle, to be built in a safe way that respects the privacy of collected data and upholds the highest data-security processes to prevent data and system breaches that could cause reputational, psychological, financial, or other harm. *(p. 15)*

3. **Humanity** — AI systems must be built using an ethical methodology grounded in fundamental human rights and cultural values, generating beneficial impact for individuals and communities and adopting a human-centric design approach that allows for human choice and determination rather than deception or manipulation. *(p. 18)*

4. **Social & Environmental Benefits** — Embraces the beneficial and positive impact of social and environmental priorities; AI systems should not cause or accelerate harm but should contribute to empowering and complementing social and environmental progress and protect both social good and environmental sustainability. *(p. 21)*

5. **Reliability & Safety** — Ensures that the AI system adheres to its specifications and behaves exactly as its designers intended (reliability) and does not pose a risk of harm to society or individuals (safety), with continuous monitoring and risk-mitigation built in. *(p. 22)*

6. **Transparency & Explainability** — AI systems must be built with a high level of clarity and explainability, and with features to track stages of automated decision-making; data, algorithms, capabilities, processes, and purpose must be transparent and explainable to those directly and indirectly affected. *(p. 24)*

7. **Accountability & Responsibility** — Holds designers, vendors, procurers, developers, owners, and assessors of AI systems — and the technology itself — ethically responsible and liable for decisions and actions that may cause risk or negative effects, and requires demonstrable human oversight, governance, and management across the entire AI System Lifecycle. *(p. 26)*

## Naming-match check vs. the project's current writeup

The project's proposal (`generate_proposal.py`) and notebook (`ai_ethics_audit.ipynb`) cite two SDAIA principles using these labels:

- "Fairness & Non-Discrimination"
- "Transparency & Explainability"

Comparison against the official 2025 document:

| Project label | Official SDAIA name | Match? |
| --- | --- | --- |
| **Fairness & Non-Discrimination** | **Fairness** (Principle 1) | **No — needs renaming.** The official principle is titled simply "Fairness." "Non-discrimination" appears in the body of the definition (the principle covers eliminating "bias, discrimination or stigmatization"), but it is not part of the principle's title. |
| **Transparency & Explainability** | **Transparency & Explainability** (Principle 6) | **Yes — exact match.** |

### Recommended fix in our writeup

Rename every occurrence of "Fairness & Non-Discrimination" to **"Fairness"** to match the SDAIA-P114E (May 2025) wording. We can keep the gloss "(non-discrimination)" in prose to preserve the substance, e.g. "the SDAIA *Fairness* principle, which requires eliminating bias, discrimination, or stigmatization in AI systems." Files to update:

- `generate_proposal.py` (line ~132)
- `ai_ethics_audit.ipynb` (cells citing the principle name, e.g. lines ~36, ~517, ~681)
- `proposal.pdf` (regenerate after the .py edit)

"Transparency & Explainability" needs no change.
