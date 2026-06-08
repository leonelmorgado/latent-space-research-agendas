# LLM-Guided Research Agenda Exploration

This folder contains a generic, case-independent version of a protocol for using a large language model (LLM) as a heuristic instrument in research agenda formation.

The protocol is meant for research teams that want to examine their own documented trajectory: publications, references, datasets, projects, technical outputs, review notes, or other traceable evidence. It does not reproduce any specific team's corpus. Each team should build its own evidence package and run the cycles with its own materials.

The folder is designed to accompany the methodological article "Exploring latent space with a GPT to support creation of research agendas in educational technology". It is intentionally generic: it provides protocol text, prompts, templates, and record structures, not the case corpus, case results, article manuscript, or author-identifying submission files.

During blind review, share this material as an exported archive without `.git/` metadata, repository remotes, author identifiers, private files, or direct links that would compromise anonymity.

## What this protocol is for

The method helps a team turn an accumulated portfolio into a discussable map of possible research directions. The LLM is used to surface relationships, assumptions, tensions, possible blind spots, candidate directions, and claims that require further scrutiny.

The useful output is not an automatic agenda. The useful output is a structured situation in which suggestions, resistances, corrections, and human decisions become visible enough to be challenged.

One important rule is to avoid letting raw internal citation counts dominate the interpretation. Self-citations and citations to close collaborators may reveal an internal intellectual trajectory, but they should not automatically outrank external theoretical influences. If a theory or concept emerged within the team, its role should be justified by its conceptual function, not by frequency alone.

## What this protocol is not

This protocol is not:

- a replacement for literature review;
- a validation procedure;
- an automated bibliometric conclusion;
- a scientific evaluator;
- a way to infer field-wide gaps from one team's portfolio;
- a substitute for expert judgement, empirical evidence, or peer review.

The LLM can propose interpretations. Researchers decide what is plausible, what is wrong, what needs evidence, and what should be discarded.

## Suggested folder structure

```text
cycles/
  00_evidence_package_template.md
  01_protocol.md
  03a_latent_state_mapping_template.md
  03b_epistemological_opportunities_template.md
  03c_contribution_potential_template.md
  04_human_consolidation_template.md
  05_external_literature_check_template.md
```

See [MANIFEST.md](MANIFEST.md) for the review/package manifest and the deliberate exclusions.

## Minimal workflow

1. Define the case: the research team, group, lab, project cluster, or other unit whose trajectory is being examined.
2. Build the evidence package: active corpus, authorship links, cited works, extracted references, classifications, exclusions, audit notes, and known data limits.
3. Run cycle 3a: map the provisional latent state of the team's trajectory.
4. Run cycle 3b: explore omissions, tensions, and epistemological opportunities.
5. Run cycle 3c: examine the contribution potential of candidate directions and clarify misconceptions.
6. Consolidate human decisions: keep, merge, reformulate, discard, or defer each candidate direction.
7. Conduct a human external literature check before treating any direction as scientifically defensible.

Only stages 3a, 3b, and 3c are LLM-facing exploratory stages. Stages 4 and 5 are human scholarly work: they can document limited AI support if used, but the decisions, appraisal of evidence, and responsibility for claims remain with the researchers.

## Documentation rule

For every LLM interaction, record:

- date and time;
- model, version, and parameters when available;
- literal prompt;
- LLM response or structured synthesis;
- human interpretation;
- human corrections and decisions;
- limitations.

Keep three layers separate:

1. what the LLM generated;
2. what the researchers interpreted;
3. what can be claimed with scientific prudence.

For Stages 4 and 5, record the human reasons for each decision, the evidence consulted, and what remains uncertain.

## Data and ethics

Use only data that the team is allowed to process and share. If the protocol is published with example materials, remove personal data, private documents, restricted PDFs, confidential project information, and any material that would compromise blind review, privacy, copyright, or institutional agreements.

For a public repository, prefer synthetic examples, public metadata, open-access sources, and clearly anonymised records.

## License

Except where otherwise noted, the original text, prompts, methodological notes, tables, templates, and original figures in this repository are licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).

Third-party materials, quoted excerpts, bibliographic records, external sources, and linked or referenced content remain under their respective licenses and terms. See [LICENSE.md](LICENSE.md).
