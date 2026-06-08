# Protocol Manifest

## Included

- `README.md`: overview, purpose, workflow, ethics, and license summary.
- `LICENSE.md`: public repository license notice.
- `cycles/00_evidence_package_template.md`: structure for assembling a case evidence package.
- `cycles/01_protocol.md`: complete five-stage protocol.
- `cycles/03a_latent_state_mapping_template.md`: prompt and record template for latent-state mapping.
- `cycles/03b_epistemological_opportunities_template.md`: prompt and record template for omissions and epistemological opportunities.
- `cycles/03c_contribution_potential_template.md`: prompt and record template for contribution potential and misconception checks.
- `cycles/04_human_consolidation_template.md`: human consolidation matrix template.
- `cycles/05_external_literature_check_template.md`: external literature check template.

## Use

This repository is a starting kit for teams that want to examine their own documented research trajectory and formulate candidate research directions. It does not contain a finished agenda. It gives the team a process for preparing evidence, asking an LLM to expose possible relationships and omissions, and then making human decisions about what is plausible, useful, risky, or premature.

To apply the protocol, copy the templates, replace placeholders with the team's own evidence package, and keep the three interpretive layers separate: model output, human interpretation, and scientifically defensible claims.

The LLM-facing exploratory stages are 3a, 3b, and 3c. Stages 4 and 5 are human scholarly work and should not be delegated to the model as final judgement.

## Using an LLM Assistant

An LLM assistant can help a team use this repository, but it should be treated as an instrument for organising and challenging the material, not as the owner of the research agenda. A useful assistant should:

- read `README.md` and `cycles/01_protocol.md` before starting;
- help the team fill `cycles/00_evidence_package_template.md` with traceable sources and clear limits;
- run or support Stages 3a, 3b, and 3c only after the evidence package and restrictions are explicit;
- keep literal prompts, model responses, human interpretation, and human decisions in separate record sections;
- flag missing evidence, overclaiming, self-citation effects, close co-authorship effects, and weakly grounded suggestions;
- refuse to treat its own output as validation, proof of a scientific gap, or a final agenda;
- leave Stages 4 and 5 to the researchers, while helping format records or organise notes if asked.

The practical test is simple: after using the repository, another reader should be able to see what the model suggested, what the researchers accepted or rejected, and what still requires literature, data, expert judgement, or empirical work.
