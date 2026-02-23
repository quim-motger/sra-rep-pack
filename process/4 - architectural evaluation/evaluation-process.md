# Architectural Evaluation: Process Description

This file documents the architectural evaluation process performed to assess whether the proposed SRA is adequately specified, representative of the target domain, and suitable for practical adoption.
It corresponds to step 4 from the ProSA-RA framework by Nakagawa et al.[^1].

In the original framework, evaluation is conceived as a structured inspection of the architectural description with stakeholders[^1]. We complement this with empirical validation and alignment strategies, following Dąbrowski et al.[^2] and Stol and Fitzgerald[^3]. Our evaluation uses a two-fold strategy: (i) **architectural alignment** — an unobtrusive analysis of a sample of existing NLP4RE tools — and (ii) **perceived technology acceptance** — a questionnaire-based survey of NLP4RE practitioners on perceived usefulness and intention to use.

## Architectural Alignment

We assessed the extent to which existing NLP4RE tools comply with the SRA by evaluating their alignment with its architectural responsibilities. Compliance indicates coverage; systematic misalignments reveal gaps.

1. We obtained a sample from the systematic survey of NLP4RE tools by Frattini et al.[^4] (126 unique tools; 62 with reachable source code). We randomly sampled 25 tools and confirmed that the distribution of key attributes (availability, RE activity, NLP task) was similar in the sample and population. Two tools were replaced after becoming unavailable.
2. We analyzed the source code of each tool to determine which architectural responsibilities from the module view each tool fulfilled (binary classification per tool–responsibility pair).
3. We prepared an annotation guideline describing each responsibility, acceptance criteria, and examples. Two authors performed a preliminary annotation on three tools; inter-annotator agreement reached substantial level (Cohen’s kappa 0.607). Disagreements were resolved by refining the guidelines. All three authors then annotated the remaining tools.

Supporting artifacts:

- [./process/4 - architectural evaluation/architectural alignment/Annotation Guidelines.pdf](/process/4%20-%20architectural%20evaluation/architectural%20alignment/Annotation%20Guidelines.pdf)
- [./process/4 - architectural evaluation/architectural alignment/evaluation matrix.xlsx](/process/4%20-%20architectural%20evaluation/architectural%20alignment/evaluation%20matrix.xlsx)
- [./process/4 - architectural evaluation/architectural alignment/traceability matrix annotations.xlsx](/process/4%20-%20architectural%20evaluation/architectural%20alignment/traceability%20matrix%20annotations.xlsx)

## Perceived Technology Acceptance

We surveyed practitioners involved in NLP4RE tool development to assess perceived usefulness, ease-of-use, and intention to use. The participant list was derived from the authors of the 126 tools in Frattini et al.[^4] (320 individuals); after exclusions (retired, no contact, co-authors), 309 practitioners remained.

The survey had five sections: (1) demographics and background (e.g. experience with design, implementation, maintenance, reuse); (2) technology acceptance — perceived ease-of-use, perceived usefulness, and intention to use, using TAM-based items[^5] and intention-to-use items from Moody[^6], on a 7-point Likert scale; (3) goal fulfillment — extent to which the SRA supports the four goals (reuse, applicability, comparability, maintainability); (4) open feedback (benefits, drawbacks, comments).

Supporting artifacts:

- [./process/4 - architectural evaluation/technology acceptance/AIRERA Documentation.docx](/process/4%20-%20architectural%20evaluation/technology%20acceptance/AIRERA%20Documentation.docx)

[^1]: Nakagawa, E. Y., et al. (2014). Consolidating a process for the design, representation, and evaluation of reference architectures. In 2014 IEEE/IFIP Conference on Software Architecture (pp. 143–152). IEEE. 
[^2]: Dąbrowski, J., et al. (2022). Mining user feedback for software engineering: Use cases and reference architecture. In IEEE 30th International Requirements Engineering Conference (RE) (pp. 114–126). 
[^3]: Stol, K.-J., & Fitzgerald, B. (2018). The ABC of Software Engineering Research. ACM Transactions on Software Engineering and Methodology, 27(3). 
[^4]: Frattini, J., Unterkalmsteiner, M., Fucci, D., & Mendez, D. (2025). NLP4RE tools: Classification, overview and management. In A. Ferrari & G. Ginde (Eds.), Handbook on Natural Language Processing for Requirements Engineering. Springer, Cham.
[^5]: Davis, F. D. (1989). Perceived usefulness, perceived ease of use, and user acceptance of information technology. MIS Quarterly, 13(3), 319–340.
[^6]: Moody, D. L. (2003). The method evaluation model: A theoretical model for validating information systems design methods. Information Systems Journal, 13(1), 79–102. 
