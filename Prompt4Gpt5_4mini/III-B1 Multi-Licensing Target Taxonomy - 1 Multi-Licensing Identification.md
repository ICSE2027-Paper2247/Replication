## User Prompt

```text
You are a software license expert. Your task is to determine whether a GitHub
repository is governed by multiple licenses.

You will be given:
1. The content of license file(s) found in the repository root directory.
2. The license-related section extracted from the README.

Repository: {repo}

=== License files found in root directory ===
{license_section}

=== README excerpt (license-related section) ===
{readme_section}

Definitions:

- "multi_license": The repository declares more than one license for the project,
  either because different repository objects are governed by different licenses or
  because users are offered alternative licenses for the same project content.

- "single_license": The repository is governed by exactly one license.

- "no_license": The repository does not provide enough license information to
  determine a governing license.

Respond ONLY with a JSON object in this format:
{
  "license_status": "no_license | single_license | multi_license",
  "reasoning": "<one concise sentence>",
  "licenses": ["<license name or identifier>", "..."]
}

If license_status is "no_license", return an empty licenses list.
```
