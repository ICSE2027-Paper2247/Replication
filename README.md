# Replication Package

This repository contains the license data, taxonomy results, and derived empirical results used in our study of non-standard licensing practices in GitHub repositories.

## Package Structure

- `Data/`: collected license-related files and repository metadata for 30,000 GitHub repositories.
- `Taxonomy/`: taxonomy results for multi-licensing targets and license terms.
- `Result/`: derived JSON/JSONL results used in the empirical analysis.
- `Validation/`: contains the manually annotated and reviewed datasets used to validate taxonomy construction, LLM-assisted consolidation, clause coverage, and multi-licensing target mapping.
- `Compatibility/`: records the rules that determine which license terms participate in compatibility analysis.
- `Prompt4Gpt5_4mini/`: contains the prompt templates used for the LLM-based tasks in this study.

## Taxonomy Results

The following figures summarize the two taxonomies constructed in the study.

![Multi-Licensing Target Taxonomy](Taxonomy/Multi-Licensing%20Target%20Taxonomy.png)

The multi-licensing target taxonomy characterizes repository objects that may be covered by different licenses, including software artifacts, textual works, media assets, hardware design artifacts, and data/model artifacts.

![License Term Taxonomy](Taxonomy/License%20Term%20Taxonomy.png)

The license term taxonomy organizes fine-grained license terms into higher-level categories and indicates whether terms are covered by standard SPDX licenses or arise from customized licenses.

## Result Files

The `Result/` directory contains the following derived data files.

| File                                       | Description                                                                                                                                                                                                                                                                                       |
| ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `spdx_license_term.jsonl`                | Full term-level annotations for standard SPDX licenses. Each line corresponds to one SPDX license and one license term, covering all 279 terms for each license. Key fields include`spdx_id`, `clause_id`, `present`, `stance`, and `evidence`.                                     |
| `custom_license_term.jsonl`              | Term-level annotations for customized or non-standard license text records. Each record corresponds to one customized license text and contains its detected present terms in`clauses`, together with metadata such as repository, license index, base SPDX information, and source labels. |
| `custom_license_texts.jsonl`             | Full extracted texts for the customized licenses used for term-level parsing and manual checking.                                                                                                                                                                                             |
| `dependency_license_compatibility.jsonl` | License compatibility analysis results for 3,000 upstream-downstream dependency pairs. Each record includes upstream/downstream license metadata, multi-licensing relationship information, conflict status, and C1/C2/C3 conflict details.                                                       |

The count of customized license text records is not the same as the repository-level count of repositories with customized license content, because a repository may contain multiple customized license texts.
