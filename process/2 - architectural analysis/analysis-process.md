# Architectural Analysis: Process Description

This file documents the architectural analysis process performed to extract system requirements, synthesize architectural requirements, and organize domain concepts.
It corresponds to step 2 from the ProSA-RA framework by Nakagawa et al.[^1].

## Extracting System Requirements

To arrive at a set of system requirements, we conducted the following steps:

1. We selected the *stakeholder focus group activity* from Frattini and Motger [^5] as a starting point for the requirements elicitation. 
2. We enhanced and complemented the requirements based on the other information sources (literature, other tools, etc.)[./process/1 - information source identification](/process/1%20-%20information%20source%20identification/Related%20Work.xlsx). For each requirement, we documented where it was elicited from in the "Source" and "Locator" columns.

The resulting set of system requirements is located in [./process/2 - architectural analysis/Requirements.xlsx](/process/2%20-%20architectural%20analysis/Requirements.xlsx) in the "System"-tab.

## Synthesizing Architectural Requirements

To arrive at a set of architectural requirements, we conducted the following steps:

1. We classified each system requirement in one of three categories (see the "Status" column of the system requirements):
    1. **covered**: The system requirement can be delegated to a reference architecture
    2. **system-only**: The system requirement only applies to an NLP4RE tool and cannot be taken care of by a software reference architecture
    3. **fundamental**: The system requirement is fundamental to the definition of an NLP4RE tool (and, therefore, not a real requirement itself)
2. We clustered all system requirements classified as **covered** and synthesized them to architecture-level requirements. These requirements pertain to a *software reference architecture of NLP4RE tools*. We support each architecture requirement with a rationale and document the trace links to system requirements in the "Source" column.

The resulting set of system requirements is located in [./process/2 - architectural analysis/Requirements.xlsx](/process/2%20-%20architectural%20analysis/Requirements.xlsx) in the "Architecture"-tab.

## Organizing Domain Concepts

To arrive at an ontology of domain concepts, we conducted the following steps:

1. We extracted relevant domain concepts from the information sources, particularly the "Domain Concepts"-notes provided by stakeholders and existing ontologies.[^3][^4]
2. We organized the domain concepts in an ontology. We are using notation conventions from UML class diagrams to represent relationships and abstractions, but also group nodes together to ease the understandability of the ontology.
3. Finally, we associate each architecture requirement with the respective domain concepts. The column "Domain Concepts" in the "Architecture" sheet of the Requirements.xlsx file lists all relevant domain concepts per requirement.

The resulting ontology of domain concepts is located in [./process/2 - architectural analysis/Domain Concepts.pdf](/process/2%20-%20architectural%20analysis/Domain%20Concepts.pdf).

[^1]: Nakagawa, E. Y., Guessi, M., Maldonado, J. C., Feitosa, D., & Oquendo, F. (2014, April). Consolidating a process for the design, representation, and evaluation of reference architectures. In 2014 IEEE/IFIP Conference on Software Architecture (pp. 143-152). IEEE.
[^2]: Lethbridge, T. C., Sim, S. E., & Singer, J. (2005). Studying software engineers: Data collection techniques for software field studies. Empirical software engineering: an international journal, 10(3), 311-341.
[^3]: Abualhaija, S., Aydemir, F. B., Dalpiaz, F., Dell'Anna, D., Ferrari, A., Franch, X., & Fucci, D. (2024). Replication in requirements engineering: the NLP for RE case. ACM Transactions on Software Engineering and Methodology, 33(6), 1-33.
[^4]: https://github.com/OpenReqEU/openreq-ontology
[^5]: Frattini, J., & Motger, Q. (2026). Towards a Software Reference Architecture for Natural Language Processing Tools in Requirements Engineering. arXiv preprint arXiv:2602.17498. https://arxiv.org/abs/2602.17498