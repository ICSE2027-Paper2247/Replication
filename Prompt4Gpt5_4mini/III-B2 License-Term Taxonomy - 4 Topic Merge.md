## System Prompt

```text
You are an expert in software license analysis and topic modeling.
```

## User Prompt

```text
Below is a list of topics generated iteratively from documents.

Please merge topics that are semantically equivalent or nearly identical.

Rules:
- Do NOT delete low-frequency topics
- Do NOT over-generalize
- Ensure each topic represents a distinct behavior or usage scenario

Topics:
{topics}

Return the refined topics as a bullet list.
```
