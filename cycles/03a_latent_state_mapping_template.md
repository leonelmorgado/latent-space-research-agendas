# Stage 3a - Latent State Mapping

Status: generic LLM-stage prompt and record template.

## Function

Ask the LLM to interpret the team's documented trajectory from the evidence package. The aim is to expose the model's dominant reading so that researchers can correct, redirect, and contextualise it.

This stage maps a provisional state. It does not identify validated gaps or final research directions.

## Evidence input

Use the evidence package recorded in `00_evidence_package_template.md`.

Add any structured summaries, tables, or files that the LLM should inspect:

- `[file or summary]`
- `[file or summary]`
- `[file or summary]`

## Guiding question

What trajectories, relationships, tensions, and theoretical anchors appear to emerge when the LLM examines the team's publications, authorship patterns, cited works, references, classifications, and documented data limits?

## Methodological restrictions

- Treat "latent state" as an operational metaphor, not as direct access to model internals.
- Separate broad bibliometric areas from theoretical anchors.
- Distinguish conceptual references from technical, instrumental, historical, endogenous, close co-authorship, or noisy references.
- Do not transform frequency into proof of scientific relevance.
- Do not infer a final agenda from this stage.

## Suggested prompt

```text
You are helping a research team explore its documented research trajectory in order to formulate candidate future research directions.

Use the evidence package provided. Map the provisional latent state of the team's trajectory.

Please identify:
1. visible trajectories;
2. strong, emerging, weak, or ambiguous relationships;
3. consolidated areas versus adjacent or peripheral areas;
4. references or concepts that may function as theoretical anchors;
5. external theoretical influences and their interpretive function;
6. internal references, self-citations, or close co-authorship signals that require substantive human reading;
7. references that appear mainly technical, instrumental, historical, or metadata noise;
8. contextual warnings needed to avoid simplistic bibliometric interpretation.

Restrictions:
- Treat "latent state" as an operational metaphor for semantic exploration, not as access to model internals.
- Do not infer validated scientific gaps.
- Do not treat citation frequency as theoretical importance without caution.
- Do not allow self-citation or close co-authorship to outrank external theoretical influence by raw volume.
- If a theoretical influence appears to emerge from inside the team, explain the conceptual function it performs rather than relying on frequency.
- Do not propose final agenda directions yet.
- Separate what the evidence suggests from what requires human judgement.

Produce:
- a provisional map;
- a table of trajectories, external theoretical influences, and possible theoretical anchors;
- relationships, tensions, and ambiguities;
- warnings about self-citation, co-authorship, metadata, and limits of reading.
```

## Record

### Date and time


### Model, version, and parameters


### Literal prompt


### LLM response or structured synthesis


### Provisional trajectory and influence map

| Visible trajectory | External theoretical influences | Internal or close-collaboration signals | Function in the map |
|---|---|---|---|
|  |  |  |  |

### Technical, historical, endogenous, or noisy references

| Reference or cluster | Type | Why it is not automatically a theoretical anchor | Follow-up needed |
|---|---|---|---|
|  | technical / historical / internal / close co-authorship / metadata noise |  |  |

### Relationships, tensions, and ambiguities

1.
2.
3.

### Human interpretation


### Human corrections, contextualisations, or decisions


### What may be claimed with scientific prudence


### Limits identified
