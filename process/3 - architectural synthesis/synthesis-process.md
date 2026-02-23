# Architectural Synthesis: Process Description

This file documents the architectural synthesis process performed to create the SRA from the architectural requirements (ARs) and domain concepts (DCs).
It corresponds to step 3 from the ProSA-RA framework by Nakagawa et al.[^1].

Nakagawa et al. propose specifying the SRA using architectural views and styles to frame the architecture from several viewpoints, including a cross-cutting, runtime, deployment, and source code viewpoint[^1].
We operationalize the viewpoints relevant to our SRA according to Clements et al.[^2] and produce the following views using UML notations:

- **Module view** — Frames the architecture from a static source-code perspective[^3]. It employs a *layered style* to specify a high-level separation of functional layers, a *decomposition style* to show the top two levels in the hierarchy of modules, and a *generalization style* to frame abstraction.

  Resulting documentation: [./process/3 - architectural synthesis/airera-module-view.pdf](/process/3%20-%20architectural%20synthesis/airera-module-view.pdf).

- **Component-and-connector views** — Frame the runtime behaviour of systems following the SRA[^4]. They are realized in two separate styles:
  - *Service-oriented-architecture (SOA) style*: organizes the runtime components as individual services (acting within their respective layer)[^5].  Resulting documentation: [./process/3 - architectural synthesis/airera-soa-view.pdf](/process/3%20-%20architectural%20synthesis/airera-soa-view.pdf).
  - *Pipe-and-filter style*: frames the core NLP processing pipeline of any NLP4RE tool[^6]. Resulting documentation: [./process/3 - architectural synthesis/airera-soa-view.pdf](/process/3%20-%20architectural%20synthesis/airera-coc-view-paf.pdf).



We compiled all views into one comprehensive architectural documentation in accordance with Bass et al.[^7], supporting all diagrams with explanations of elements and relations.
The third author, an expert in software architecture with experience both in academia and industry, reviewed, assessed, and finalized the SRA documentation.

[^1]: Nakagawa, E. Y., Guessi, M., Maldonado, J. C., Feitosa, D., & Oquendo, F. (2014, April). Consolidating a process for the design, representation, and evaluation of reference architectures. In 2014 IEEE/IFIP Conference on Software Architecture (pp. 143-152). IEEE.
[^2]: Clements, P., Bachmann, F., Bass, L., Garlan, D., Ivers, J., Little, R., ... & Stafford, J. (2011). Documenting software architectures: views and beyond (2nd ed.). Addison-Wesley.
[^3]: Hofmeister, C., Nord, R., & Soni, D. (1999). Describing software architecture with UML. In Proceedings of the 1st Working IFIP Conference on Software Architecture (WICSA1) (pp. 145-159). Springer.
[^4]: Garlan, D. (2003) Formal modeling and analysis of software architecture: Components, connectors, and events. In International School on Formal Methods for the Design of Computer, Communication and Software Systems. (pp. 1–24). Springer.
[^5]: Laskey, K. B. & Laskey, K. (2009) Service oriented architecture. Wiley Interdisciplinary Reviews: Computational Statistics. vol. 1, no. 1 (pp. 101–105).
[^6]: Rohnert, H. (1996). Pattern-oriented software architecture. In Proceedings of the 2nd USENIX Conference on Object-Oriented Technologies and Systems (COOTS '96). USENIX Association.
[^7]: Bass, L., Clements, P., & Kazman, R. (2012). Software architecture in practice (3rd ed.). Addison-Wesley.
