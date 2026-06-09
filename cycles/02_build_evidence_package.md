# Stage 2 - Build the Evidence Package

Stage 2 turns a team's publication trail into evidence that an LLM can inspect. The team provides the corpus, the boundaries, and the permissions, an AI assistant can help collect, normalise, extract, compare, and document the material.

The result should be an evidence package that is good enough to support Stage 3a: a traceable map of what was included, where it came from, what was extracted, and what is missing.

Use `00_evidence_package_template.md` to record the final package. This page explains how to build it.

## 1. Define the Team and the Boundary

Start by naming the unit being examined. It may be a personal career, research team, lab, centre, project cluster, doctoral cohort, or another group with a documented trajectory.

Record:

- the team members or authors considered part of the case;
- known name variants, ORCID identifiers, institutional profiles, or other author identifiers;
- the time span covered;
- the types of publication included;
- the types of publication excluded;
- the reason for the exploration, such as strategic renewal, agenda formation, interdisciplinary integration, or review of a research trajectory.

This scope boundary matters because every later distinction depends on it. A cited work may be external in one team's package and internal in another. A publication may be part of the active corpus for one case and contextual background for another.

## 2. Choose the Entry Route

There are two common ways to start. A team can use one or both.

### Route A - Direct PDF Folder

The team provides a folder containing the PDFs that should form the active corpus.

Use this route when the team has a curated local collection or when online metadata is incomplete. The assistant can then:

- list the files;
- extract titles, authors, years, DOIs, abstracts, and reference sections where possible;
- identify in-text citation contexts;
- compare extracted metadata with online sources such as OpenAlex, Crossref, institutional repositories, or publisher pages;
- flag unreadable PDFs, duplicates, missing metadata, and uncertain matches.

This route gives the team strong control over inclusion, but it requires attention to copyright and access rights. Only process and share files that the team is allowed to use for this purpose.

### Route B - Online Author or Publication Sources

The team provides ORCID identifiers, institutional profile pages, DOI lists, repository links, Scopus or Web of Science exports, Google Scholar profiles, Zotero libraries, BibTeX files, RIS files, or other online sources.

Use this route when the team wants the assistant to help collect or reconstruct the publication list. The assistant can then:

- retrieve or reconcile publication metadata;
- use sources such as OpenAlex to identify authorship, works, venues, years, DOIs, and referenced works;
- look for open-access PDF links or repository copies when legally available;
- deduplicate records across sources;
- flag uncertain authorship, ambiguous names, missing DOIs, and records that require human checking.

This route is faster when identifiers are good. It is weaker when names are ambiguous, author profiles are incomplete, or online sources miss local publications.

## 3. Build the Active Publication Corpus

The active corpus is the set of works that represents the team's trajectory for this protocol. Not everything the team has ever written is automatically considered: only the set that the team is willing to treat as evidence for the exploration.

For each publication, record as much as possible:

- stable identifier, such as DOI, OpenAlex work ID, repository handle, or local file name;
- title;
- year;
- venue;
- authors;
- team members linked to the publication;
- source of the record;
- PDF availability and legal access status;
- inclusion or exclusion decision;
- notes on uncertainty.

If multiple sources disagree, keep the disagreement visible. Do not silently merge uncertain records.

## 4. Extract Authorship and Team Links

Create a table that connects team members to publications. If online identifiers are available, keep them. If names must be matched manually, record the rule used.

Useful outputs:

- one table of team members and identifiers;
- one table of publications;
- one table of author-publication links;
- one audit note for ambiguous names, name changes, initials, homonyms, and institutional moves.

This step is boring in the best possible way: it prevents later interpretive drama. If the team boundary is unstable, the LLM will treat noise as signal.

## 5. Extract Cited Works and Reference Material

The evidence package can use two complementary layers.

### Metadata Citation Layer

Sources such as OpenAlex can provide cited works or referenced works for many publications. This layer is useful for building a citation graph:

- publication in the active corpus;
- cited work;
- cited work authors;
- cited work year;
- cited work venue;
- DOI or OpenAlex ID when available;
- citation edge between the corpus publication and the cited work.

This layer is often broad and structured, but incomplete. It may miss references, inherit metadata errors, or fail to capture how a work is used in the text.

### PDF and Textual Reference Layer

When the team has legal access to PDFs or full text, the assistant can extract reference sections and in-text citation contexts. This layer helps answer a different question: not only what was cited, but how it appears in the team's writing.

Useful outputs:

- extracted reference list items;
- matched references to DOI, OpenAlex ID, or other identifiers when possible;
- in-text citation strings;
- nearby sentence or paragraph context;
- section where the citation appears, if detectable;
- match confidence;
- extraction errors and unresolved references.

Do not treat extraction as perfect. PDF parsing can break on columns, footnotes, scanned pages, broken ligatures, and unusual reference styles. Keep an error log.

## 6. Distinguish External, Internal, and Close-Collaboration References

The protocol needs to avoid a simple frequency trap. A frequently cited work may be central, but it may also be internal continuity, a technical tool, a method everyone uses, or a consequence of close co-authorship.

Classify cited works with at least these categories:

- external to the team;
- authored by one or more team members;
- authored by close collaborators or frequent co-authors;
- mixed authorship;
- uncertain.

The classification should use explicit rules. For example:

- mark a cited work as internal if any cited-work author matches a team member identifier or a confirmed name variant;
- mark it as close-collaboration if the cited-work author has repeated co-authorship with the team in the active corpus or in the wider metadata;
- mark it as uncertain when names match weakly or identifiers are missing.

This classification does not decide theoretical importance. It only protects Stage 3a from treating internal density as external influence.

## 7. Identify Use Within the PDFs

If full text is available, ask the assistant to look at citation use, not just citation presence.

For each cited work or cluster, try to record:

- where it appears, such as introduction, theory, method, results, discussion, or technical description;
- whether it is used as a conceptual anchor, method reference, empirical comparison, technical tool, historical background, policy reference, or passing mention;
- whether it supports a claim, frames a problem, defines a concept, justifies a method, or only appears in a list;
- short citation contexts when legally and ethically usable;
- uncertainty in the classification.

This step is where the evidence package becomes more useful than a citation count. It gives Stage 3a material for distinguishing theoretical influence from technical or historical background.

## 8. Create the Evidence Summary for the LLM

Before Stage 3a, prepare a compact summary that an LLM can read alongside the structured files.

Include:

- what the case is;
- what the active corpus contains;
- how the corpus was built;
- which sources were used;
- how authorship was matched;
- how cited works were extracted;
- how internal, external, and close-collaboration references were classified;
- which PDFs or full texts were inspected;
- what remains incomplete or uncertain;
- what the LLM is allowed to infer;
- what the LLM must not infer.

The summary should be clear enough that another researcher or another assistant could understand the package without guessing the hidden decisions.

## 9. Suggested Files

The exact filenames do not matter, but the package should make the evidence inspectable. A practical structure is:

```text
evidence/
  evidence_package_summary.md
  publications.csv
  team_members.csv
  author_publication_links.csv
  cited_works.csv
  citation_edges.csv
  extracted_references.csv
  in_text_citation_contexts.csv
  reference_classification.csv
  exclusions.csv
  audit_notes.md
  extraction_errors.md
```

For a small team, spreadsheets may be enough. For a large corpus, use CSV, JSON, database exports, or scripts. What matters is traceability.

## 10. Prompt for an AI Assistant

Use or adapt this prompt when asking an assistant to help build Stage 2.

```text
You are helping a research team build an evidence package for LLM-guided research agenda exploration.

The aim is to prepare traceable evidence for Stage 3a, not to interpret the team's future agenda yet.

Use the publications, PDFs, ORCID identifiers, metadata exports, online sources, and constraints provided by the team. Where appropriate, use bibliographic sources such as OpenAlex to reconcile publication records, authorship, cited works, and citation edges. If PDFs or full text are legally available, extract reference lists and in-text citation contexts, but record parsing errors and uncertainty.

Produce:
1. an active publication corpus;
2. team member and author-publication link tables;
3. cited works and citation edge tables;
4. extracted reference and in-text citation context tables when full text is available;
5. a classification of cited works as external, internal, close-collaboration, mixed, or uncertain;
6. an exclusions and uncertainty log;
7. an evidence package summary for Stage 3a.

Restrictions:
- Do not treat metadata completeness as evidence of scientific importance.
- Do not infer field-wide gaps from this corpus.
- Do not treat citation frequency as theoretical influence.
- Do not bypass copyright, access restrictions, privacy constraints, or platform terms.
- Separate what was retrieved, what was inferred, what was manually corrected, and what remains uncertain.
```

## Ready for Stage 3a

The package is ready when the team can say, plainly:

- these are the works we included;
- these are the works we excluded;
- these are the sources and extraction methods we used;
- these are the authors and identifiers we matched;
- these are the cited works and citation contexts we could recover;
- these are the internal, external, and close-collaboration signals;
- these are the limits that must constrain the LLM.

If any of those sentences is impossible to complete, Stage 2 is not finished. The team can still proceed, but the missing pieces must travel forward as visible limits.
