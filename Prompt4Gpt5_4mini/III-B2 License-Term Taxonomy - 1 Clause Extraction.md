## System Prompt

```text
You are an OSS license expert.
```

## User Prompt

```text
Task: Decompose the following license text into a list of atomic action-based terms.

Instructions:
- Identify unique atomic terms with actions described in the text, focusing only on actionable expressions.
- For each atomic term, extract its original text and summary. The exact original text snippet **copied verbatim** from the text, without modification, rewording, or paraphrasing, and it must contain **at least one complete sentence**. Write the summary as a concise, standardized verb phrase that states the action and the minimum necessary object/scope(), so that it can stand alone as a clear, readable, and actionable clause.
- Each extracted unit should express only one distinct action.
- The summary shall exclude any modal or attitude (e.g., can, shall, must, may, permit, deny, not) and keep only the plain action meaning.
- Directly extract boilerplate clauses (e.g., 'Entire Agreement Clause', 'No Waiver Clause', 'Survival Clause', 'Severability Clause').
- Strictly exclude all explanatory or non-actionable texts, including copyright notices, component or path lists, definitions or explanations of terms, software usage instructions, descriptive or editorial statements, and any content without substantive legal or license clause significance, as well as all actions or obligations unrelated to either the Licensor or the Licensee.

Return the result strictly in valid JSON format:
[
  { "Summary": "...", "original text": "..." },
  { "Summary": "...", "original text": "..." }
]

{retry_hint}
License text:
{license_text}
```
