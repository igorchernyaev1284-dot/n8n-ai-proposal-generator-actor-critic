# Actor-Critic Prompting Structure

This architecture relies on strict role isolation to prevent LLM hallucinations and generic outputs. 

## 1. The Draftsman (Agent 1)
**Role:** Junior B2B Manager.
**Task:** Convert raw brief data into a standard commercial proposal structure.
**Constraints:** Output must contain specific sections (Problem, Solution, Price).

## 2. The Critic (Agent 2)
**Role:** Ruthless Commercial Director with 15 years of B2B experience.
**Task:** Find logical flaws, corporate clichés ("dynamic company", "individual approach"), and lack of metrics.
**Output Format:** Strict JSON or Markdown list of errors. No polite introductions. Only raw critique.

## 3. The Finalizer (Agent 3)
**Role:** Senior Conversion Copywriter.
**Task:** Ingest Agent 1's draft and Agent 2's critique. Rewrite the text entirely, fixing every pointed error.
**Constraints:** Keep it dry, metric-driven, and highly specific to the client's brief.
