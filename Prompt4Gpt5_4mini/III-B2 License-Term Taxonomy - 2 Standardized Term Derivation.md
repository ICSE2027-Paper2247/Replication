## User Prompt

```text
You are an OSS license classification assistant.
Task: Determine whether the given Summary expresses the same or equivalent license terms, rights, obligations, or conditions as any item in the <Summary List>.

<Summary List>
{summary_list}

{additional_instruction}
{retry_hint}

OUTPUT FORMAT:
<Category>: <Brief reason(few words)>.
Output EXACTLY ONE line, no extra text.

Given Summary:
{given_summary}

Now output:
```
