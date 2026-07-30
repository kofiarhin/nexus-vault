# Registry Schema

## Project Registry

Required columns:

| Column | Meaning |
|---|---|
| ID | Stable lowercase project identifier |
| Name | Human-readable project name |
| Status | Current lifecycle label |
| Path | Vault-relative path to project `INDEX.md` |
| Updated | ISO date of material registry change |

Parsers must ignore Markdown headings, explanatory prose, the separator row, and blank rows. A missing registry is a controlled error; an empty data section is a valid empty result.

## Document Registry

Document identifiers must be stable, paths must be Vault-relative, and entries must point to canonical documents rather than generated duplicates.
