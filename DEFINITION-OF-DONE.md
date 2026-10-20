# Definition of Done — Submission Requirements (With AI / Without AI)

How to submit each assignment and what qualifies as strong work. The review takes approximately five minutes; `DEFENSE.md` is the review entry point.

## REQUIRED ARTIFACTS (for every assignment)

- `spec.md` (≤ 1 page): intent, entities/steps, and acceptance criteria. If AI is used, specify the task for the AI. Acceptance criteria must be recorded in a commit, not only in `DEFENSE.md`.
- A model artifact + one rendered diagram (Mermaid / PlantUML).
- An audit of the top three discrepancies (model ↔ spec ↔ previous models) and their corrections through changes to the spec/acceptance criteria, rather than manual patches.
- `DEFENSE.md` (1 page): the review entry point.
- An ADR for key decisions, following MADR.

## `DEFENSE.md` TEMPLATE

1. **Intent and criteria:** 1–2 sentences.
2. Top three discrepancies found and fixed (against the spec item) → commit link.
3. **Key decision:** explain which alternatives were considered and why one was chosen (`adr/...`).
4. **Verification:** explain how consistency with the previous model was checked.

## CROSS-CUTTING REQUIREMENT

Keep the model chain consistent: data → requirements → interaction → process → architecture. Each assignment builds on previous assignments and must not contradict them.

## TWO WORKFLOWS

- **Without AI:** the evidence trail consists of your decision history and your self-check of the first version against the spec.
- **With AI:** additionally maintain a complete prompt trail (`ai/`) and audit the AI output by identifying and correcting the top three errors you found. For each discrepancy: link to the prompt, feedback comment, and additional spec clause/criterion.

Both workflows have the same quality bar and review budget. Understanding and being able to defend decisions is assessed, not the tool used.

## “DONE” CHECKLIST

`DEFENSE` (1 page) · `spec` (≤ 1 page) with acceptance criteria · top three discrepancies with commits · artifact + rendered diagram through commits · ADR · realistic Git history · clean repository.

The instructor will provide the full versions — `DEFINITION-OF-DONE.md` and `DEFINITION-OF-DONE-NO-AI.md` — in the course repository.
