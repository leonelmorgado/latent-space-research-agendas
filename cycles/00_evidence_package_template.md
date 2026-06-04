# Stage 2 - Evidence Package Template

Status: not yet completed.

This file records the evidence that will be provided to the LLM before the exploratory cycles. It should describe the team's corpus and its limits. It should not contain results from the LLM cycles.

## Case definition

| Item | Description |
|---|---|
| Team or unit examined | `[Describe the research team, lab, project group, or other unit.]` |
| Purpose of the exploration | `[Explain why the team is exploring its trajectory: agenda formation, renewal, strategic reflection, interdisciplinary integration, etc.]` |
| Time span covered | `[Years covered by the evidence.]` |
| Domain or domains | `[Research field(s), without overstating representativeness.]` |
| Inclusion logic | `[What counts as part of the corpus.]` |
| Exclusion logic | `[What was excluded and why.]` |

## Core evidence

| Element | Local file or source | Status |
|---|---|---|
| Active publication corpus | `[path or source]` | `[available / pending / incomplete]` |
| Team authors and author-publication links | `[path or source]` | `[available / pending / incomplete]` |
| Cited works or references | `[path or source]` | `[available / pending / incomplete]` |
| Extracted reference lists from full texts, when legally available | `[path or source]` | `[available / pending / incomplete]` |
| Classification of cited works, authors, topics, or areas | `[path or source]` | `[available / pending / incomplete]` |
| External influence summaries | `[path or source]` | `[available / pending / incomplete]` |
| Authorship audit | `[path or source]` | `[available / pending / incomplete]` |
| Exclusions and rejected attributions | `[path or source]` | `[available / pending / incomplete]` |
| Data quality notes | `[path or source]` | `[available / pending / incomplete]` |

## Evidence summary

Use this section to summarise the evidence without interpreting it as a result.

- Number of active records:
- Time span:
- Number of team members or configured authors:
- Number of cited works or references:
- Number of extracted reference items, if applicable:
- Main metadata sources:
- Main data cleaning steps:
- Known anomalies:

## Limits of the package

Record limits before running the LLM cycles.

- The corpus documents this team's trajectory; it does not represent the whole field.
- Co-occurrence, citation frequency, and bibliometric density do not prove scientific gaps.
- Missing metadata may hide or distort relationships.
- Self-citation and close co-authorship may inflate apparent theoretical influence.
- Legal or access restrictions may limit full-text inspection.
- The LLM must not be treated as a final scientific judge.

## Ready to proceed?

The evidence package is ready for Stage 3a when the team can provide the LLM with:

- a concise corpus summary;
- the relevant source files or structured summaries;
- data quality warnings;
- known exclusions;
- methodological restrictions;
- a clear statement of what the LLM is allowed and not allowed to infer.
