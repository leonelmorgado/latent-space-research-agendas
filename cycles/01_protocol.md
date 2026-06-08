# Protocol for LLM-Guided Research Agenda Exploration

## Objective

Use an LLM as a heuristic instrument to help a research team examine its documented trajectory and formulate candidate research directions.

The protocol is designed to surface possible relationships, tensions, assumptions, omissions, and contribution paths. It does not validate scientific claims. It creates a structured record that researchers can criticise, revise, and consolidate.

## Layers to keep separate

1. Case: the team, lab, project group, or research unit being examined.
2. Evidence: publications, references, metadata, classifications, audits, exclusions, datasets, or other traceable records.
3. LLM: semantic exploration instrument.
4. Researchers: conduct, correct, interpret, and decide.
5. Output: methodological report, agenda memo, article section, or internal strategy document.

## Stages

Only Stages 3a, 3b, and 3c are LLM-facing exploratory stages. Stages 4 and 5 are human decision and appraisal stages. They may document limited AI support, but the protocol must not let the model decide what should enter the team's agenda or what the literature validates.

### Stage 1 - Starting point

Define the team, its documented trajectory, and the practical reason for exploring possible research directions.

### Stage 2 - Evidence package

Assemble the evidence that will be provided to the LLM. Record data sources, inclusion and exclusion criteria, metadata quality, and known limits.

### Stage 3a - Latent state mapping

Ask the LLM to map the provisional state it infers from the evidence.

The goal is to expose the dominant interpretation the model forms when it sees the team's trajectory, so that researchers can correct, redirect, or contextualise it.

Expected output:

- provisional map of the team's trajectory;
- candidate theoretical anchors;
- external theoretical influences and their interpretive function;
- separation between external theoretical influence, internal continuity, technical infrastructure, historical background, and metadata noise;
- strong, weak, and emerging relationships;
- technical, instrumental, historical, endogenous, or noisy references;
- warnings about metadata, self-citation, co-authorship, and overinterpretation.

### Stage 3b - Omissions and epistemological opportunities

Ask the LLM to explore possible omissions, blind spots, tensions, or under-operationalised concepts.

Expected output:

- candidate omissions or opportunities;
- possible research directions;
- theoretical focus supporting each direction;
- what evidence is missing;
- what should be reformulated or stopped.

### Stage 3c - Contribution potential and misconception check

Ask the LLM to examine what each candidate direction could contribute and what claims should be avoided.

Contribution categories:

- conceptual;
- methodological;
- technological;
- empirical;
- organisational.

Expected output:

- contribution potential for each candidate direction;
- required evidence, data, or artefacts;
- feasibility with the team's existing trajectory;
- risk of overclaiming;
- misconceptions and terms to avoid.

### Stage 4 - Human consolidation

Researchers decide what to keep, merge, reformulate, discard, or defer.

The protocol itself must not be listed as a candidate direction for the team. Candidate directions should be substantive and connected to the team's trajectory.

This is not an autonomous LLM generation cycle. Its output is a human-consolidated matrix with reasons for each decision.

### Stage 5 - External literature check

Consolidated directions are checked against literature outside the team. This step controls endogeneity and helps decide whether to maintain, reformulate, discard, or return to an earlier stage.

This is a human scholarly check, not a prompt that asks the LLM to validate the directions. The LLM may help organise search notes or summaries only if the researchers verify sources and decisions themselves.

## Required record

Each LLM stage should record:

- date and time;
- model, version, and parameters when available;
- literal prompt;
- LLM response or structured synthesis;
- human interpretation;
- human corrections and decisions;
- limitations.

Stages 4 and 5 should also record human reasons, literature or evidence consulted, directions maintained or rejected, and remaining uncertainty.

## Methodological restrictions

- Treat "latent space" as an operational metaphor for semantic exploration, not as direct access to the model's internal vectors.
- Do not turn frequent areas into scientific gaps.
- Do not treat citation frequency as theoretical importance without human reading.
- Distinguish theoretical anchors from technical tools, methods, historical background, self-citation, close co-authorship, and metadata noise.
- Do not allow self-citation or close co-authorship to outrank external theoretical influence by raw volume.
- If an internally produced work functions as a theoretical anchor, justify that role by its conceptual function in the team's trajectory, not by citation frequency alone.
- Do not infer a final research agenda from one LLM response.
- Check any direction against external literature before presenting it as scientifically defensible.

## Success criterion

The process succeeds when it creates a traceable, criticisable, human-consolidated set of candidate directions and the reasons for accepting, reformulating, postponing, or rejecting them.
