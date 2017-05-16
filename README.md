These diagrams are an exploration of the
[ORES](https://meta.wikimedia.org/wiki/Objective_Revision_Evaluation_Service)
architecture, from a slightly idealized perspective.  Most are data flow
diagrams, giving a high-level overview of interactions between components.

Contents
===

Data flow diagrams
---
* `context` - Highest-level overview of ORES.
* `level 1` - Communication between main subsystems.
* `wikilabels` - The manual keying system.
* `scoring` - Running models against incoming revisions.
* `metrics` - Flow of data from subsystems towards our metrics aggregator.
* `training` - How models are created

Other
---
* `use_cases` - Rough overview of how ORES is used.
* `ores_class` - Rough ERD of Python classes.
* `ores_proposed_threading`, `ores_proposed_threading_precached`, `ores_mutex_success` - Potential mutex design to simplify work tracking.

Building
===

Diagrams are either written in LaTeX or using ArgoUML.  To compile the .tex into .pdf,

  latexmk -pdf
