# Designing a Software Reference Architecture for NLP4RE Tools

<!--[[GitHub](https://img.shields.io/github/license/airera/study-sra)](./LICENSE)-->
<!-- [![DOI](https://zenodo.org/badge/702902445.svg)](https://zenodo.org/doi/10.5281/zenodo.10423665)
[![arXiv](https://img.shields.io/badge/arXiv-2401.01154-b31b1b.svg)](https://arxiv.org/abs/2401.01154) -->

This repository contains the replication package for the study designing a software reference architecture (SRA) for natural-language processing (NLP) based requirements engineering (RE) tools (NLP4RE).
The design follows the ProSA-RA process by Nakagawa et al.[^1].

> [!important]
> This repository currently contains only early results of the SRA creation framework. 
> Early results include the elicitation of requirements from NLP4RE stakeholders involved in a focus group activity.
> The remaining steps are future work of the current research preview.

![Overview of the SRA creation framework](figures/airera-roadmap.png)

## Author and Article Details

The following authors were involved in the study.

| Name | Affiliation | Contribution |
|---|---|---|
| Julian Frattini | Chalmers University of Technology, Sweden | Shared first author |
| Quim Motger | Universitat Politècnica de Catalunya, Spain | Shared first author |

Contact the corresponding authors via https://julianfrattini.github.io/ and https://quim-motger.github.io/.

*Cite this work as:* Frattini, J., and Motger, Q. Towards a Software Reference Architecture for Natural Language Processing Tools in Requirements Engineering. _Under Review_.[^2]

## Description of Artifacts

This repository contains the following files:

```
├── figures: all data used in this study
│   ├── airera-roadmap.pdf : illustration of the applied research method (pdf)
│   └── airera-roadmap.png : illustration of the applied research method (png)
├── process : material for the SRA creation process following Nakagawa et al.
│   ├── 1 - information source identification : elicitation of potential sources of requirements
│   │   ├── stakeholders : elicitation of requirements from NLP4RE tool users and developers
│   │   │   ├── Group 1 Functional Requirements : elicited functional requirements
│   │   │   ├── Group 2 Non-Functional Requirements : elicited non-functional requirements
│   │   │   ├── Group 3 Domain Concepts : elicited domain concepts
│   │   │   ├── Group 4 GenAI Challenges : elicited challenges and constraints particular to GenAI
│   │   │   ├── AIRE'25 Interactive Session Instructions.pptx : slides to introduce the interactive session at the AIRE'25 workshop to elicit requirements
│   │   │   └── AIRE'25 Results.pdf : formalization of the results from the four groups
│   │   └── Related Work.xlsx : tabular overview of related scientific manuscripts
│   └── 2 - architectural analysis : extraction of requirements from the identified sources
│       ├── analysis-process.md : process description of the architectural analysis
│       └── Requirements.xlsx : system requireents elicited from the focus group activity
└── LICENSE.md : license file clarifying reuse of this material
```

## Usage

Depending on your use case, consult the following files:

- **Replicating the focus group activity**: If you want to replicate the elicitation of requirements from NLP4RE stakeholders, access the *AIRE'25 Interactive Session Instructions.pptx* file that explains the method. For our implementation at AIRE'25, we invited participants to place post-it notes on white boards.
- **Reviewing the architectural analysis**: If you want to review the extraction of requirements from the information sources, access the *Requirements.xlsx* file. In the "System"-tab, you find the requirements in and rationale for them in respective columns. The "Source" and "Locator" columns specify, where this requirement was extracted from. In the *analysis-process.md* file you find a description of the applied extraction and synthesis process.
- **Accessing the requirements**: If you want to check the requirements that we arrived at, review the *Requirements.xlsx* file. 

## License

Copyright © 2025 Julian Frattini and Quim Motger.
This work is licensed under [MIT License](./LICENSE).

[^1]: Nakagawa, E. Y., Guessi, M., Maldonado, J. C., Feitosa, D., & Oquendo, F. (2014, April). Consolidating a process for the design, representation, and evaluation of reference architectures. In 2014 IEEE/IFIP Conference on Software Architecture (pp. 143-152). IEEE.
[^2]: Use the "Cite this Repository"-function on GitHub based on the CITATION.cff file.