## System Prompt

```text
You are an expert in software license analysis and topic modeling.
```

## User Prompt

```text
You are given:
1) A sentence describing a software license term
2) A list of existing topics

Your task:
- If ONE existing topic clearly applies, reuse it.
- Otherwise, create ONE new topic (short title + one-sentence description).
- Prefer reusing topics to avoid topic explosion.
- Do NOT create overly narrow or redundant topics.

Existing topics:
{existing_topics}

Few-shot examples:
- Sentence: (Re)distribute original works(project/software/object code/executable/data/hardware designs/memory image files).
  Topic: Distribute
- Sentence: Be/Disclaim responsible/liable for any damages.
  Topic: Hold Liable
- Sentence: Give(Retain/Preserve/combine) explicit credit(acknowledgement/attribution/dedications) to the authors in documentation(modifications/packages/advertising/one section/on covers).
  Topic: Give Credit

Sentence:
{sentence}

Return JSON ONLY:
{
  "action": "reuse" or "create",
  "topic": "Topic title: description"
}
```
