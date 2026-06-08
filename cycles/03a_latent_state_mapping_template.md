# Stage 3a - Latent State Mapping

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

Record when the interaction took place or when the synthesis was produced. Include timezone if this matters for later comparison.

### Model, version, and parameters

Identify the LLM, product, model name or version, and any visible settings such as temperature, reasoning mode, tools, retrieval sources, or system constraints.

### Literal prompt

Paste the exact prompt given to the LLM. If files or tables were attached, name them and point to their stored location.

### LLM response or structured synthesis

Preserve the full response, or write a structured synthesis if the full transcript is stored elsewhere. Do not mix human evaluation into this section.

### Provisional trajectory and influence map

Use this table to record the model's proposed map of visible trajectories, influence clusters, and the function it assigns to each one.

| Visible trajectory | External theoretical influences | Internal or close-collaboration signals | Function in the map |
|---|---|---|---|
|  |  |  |  |

### Technical, historical, endogenous, or noisy references

Use this table to separate references that may appear important by frequency or proximity but should not automatically be treated as theoretical anchors.

| Reference or cluster | Type | Why it is not automatically a theoretical anchor | Follow-up needed |
|---|---|---|---|
|  | technical / historical / internal / close co-authorship / metadata noise |  |  |

### Relationships, tensions, and ambiguities

List the relationships, tensions, and ambiguous signals that need human reading before they can become claims or candidate directions.

1.
2.
3.

### Human interpretation

Record what the researchers think the model has usefully surfaced, misunderstood, overemphasised, or missed.

### Human corrections, contextualisations, or decisions

Record corrections to the model's reading, contextual information not visible in the evidence package, and decisions about what should guide Stage 3b.

### What may be claimed with scientific prudence

Write only the cautious claims that can be supported after this stage. Avoid claims about validated gaps, final priorities, or field-wide conclusions.

### Limits identified

Record limits of the evidence package, model response, metadata, terminology, coverage, or human interpretation that should constrain later stages.
