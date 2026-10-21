# TDT4250 Model-Driven Software Engineering

[← All courses](../readme.md)

> **Link types:** 📝 starts a quiz · 📖 opens reading material (lecture notes, course pages, external sites)

[![Model-Driven Development](https://img.shields.io/badge/MDD%2FMDA-455A64?style=for-the-badge&logo=eclipseide&logoColor=white)](https://www.ntnu.edu/studies/courses/TDT4250)
[![Eclipse EMF](https://img.shields.io/badge/Eclipse%20EMF-2C2255?style=for-the-badge&logo=eclipseide&logoColor=white)](https://en.wikipedia.org/wiki/Eclipse_Modeling_Framework)
[![UML](https://img.shields.io/badge/UML-FBB034?style=for-the-badge&logoColor=black)](https://en.wikipedia.org/wiki/Unified_Modeling_Language)
[![Software Product Lines](https://img.shields.io/badge/Software%20Product%20Lines-9C27B0?style=for-the-badge&logoColor=white)](https://en.wikipedia.org/wiki/Software_product_line)

**Content:**
- Introduction to meta-programming and meta-modelling
- Domain-specific languages (DSLs), syntax and semantics
- Model-driven development of software: transformations and code generation
- Constraints and queries in models (e.g. OCL)
- Component-based development and architectures
- Software product lines: variability at design time and run time
- Deployment, frameworks and continuous integration of modular systems

**Learning outcomes:**
- **Knowledge:** general methods for modelling, designing and implementing modular software; principles of model-driven development
- **Skills:** practical ability to model, design and implement modular software using modern frameworks and model-based techniques
- **General competence:** selecting appropriate methods and techniques for developing modular and model-driven software systems

## Contents

- [Part 1 – Introduction to MDE](#part-1--introduction-to-mde)
- [Part 2 – Software product lines](#part-2--software-product-lines)
- [Part 3 – Variability implementation](#part-3--variability-implementation)
- [Part 4 – Variability with parameters](#part-4--variability-with-parameters)
- [Part 5 – Domain-specific languages](#part-5--domain-specific-languages)
- [Part 6 – MOF and Model-Driven Architecture](#part-6--mof-and-model-driven-architecture)
- [Part 7 – Eclipse Modeling Framework and Ecore](#part-7--eclipse-modeling-framework-and-ecore)

## Quizzes

### Part 1 – Introduction to MDE

*Based on Lecture 1, 📖 [Schmidt 2006](https://ieeexplore.ieee.org/document/1610613) and 📖 [Whittle et al. 2014](https://ieeexplore.ieee.org/document/6824042).*

📝 **Quiz:** [Model-Driven Development – Part 1](https://dev-quizmachine.itautomasjon.no/Quiz/Take/modeldrivendev1) · [FlexiQuiz version](https://www.flexiquiz.com/SC/N/ModelDrivenDev1)

| Topic | Details |
|---|---|
| Models + Transformations = Artifacts             | DSLs (SQL, HTML, Kubernetes YAML, Regex)                |
| CASE tools vs. MDE                               | Why CASE failed in the 80s                              |
| Metamodels: "model of models"                    | Legend/map analogy                                      |
| DSL vs GPL                                       | Examples and differences                                |
| Industrial use of MDE (Whittle 2014)             | Partial system generation, architecture documentation   |
| Benefits beyond code generation                  | Explicit architectures, separation of concerns           |
| Adoption strategies                              | Bottom-up (developer-led) vs. top-down mandates         |
| Models ≠ Reality                                 | Abstraction, assumptions, purpose                       |
| Correct-by-construction                          | Contrast with construct-by-correction                   |
| MDE in domain-focused companies                  | Automotive, printers, finance vs. consultancies         |

[↑ Back to top](#tdt4250-model-driven-software-engineering)

### Part 2 – Software product lines

*Based on Lecture 2 and 📖 [Apel et al. 2013, Feature-Oriented Software Product Lines](https://link.springer.com/book/10.1007/978-3-642-37521-7).*

📝 **Quiz:** [Model-Driven Development – Part 2](https://dev-quizmachine.itautomasjon.no/Quiz/Take/modeldrivendev2)

| Topic | Details |
|---|---|
| Definition of SPL                                | Family of products sharing core assets + controlled variability |
| Features                                         | User-visible functionality, building blocks for variability      |
| Domain vs Application Engineering                | For reuse (platform) vs with reuse (products)                   |
| Adoption strategies                              | Proactive, Extractive, Reactive – pros/cons                     |
| Feature modeling basics                          | Mandatory, optional, OR, XOR groups                             |
| Constraints in feature models                    | Example: MST ⇒ Undirected ∧ Weighted                            |
| Benefits of SPL                                  | Reduced cost, faster time-to-market, improved quality            |

[↑ Back to top](#tdt4250-model-driven-software-engineering)

### Part 3 – Variability implementation

*Based on Lecture 3 and 📖 [Apel et al. 2013, Feature-Oriented Software Product Lines](https://link.springer.com/book/10.1007/978-3-642-37521-7).*

📝 **Quiz:** [Model-Driven Development – Part 3](https://dev-quizmachine.itautomasjon.no/Quiz/Take/modeldrivendev3)

| Topic | Details |
|---|---|
| Binding times                                    | Compile-time, load-time, run-time                               |
| Language-based mechanisms                        | Parameters, design patterns, frameworks, components             |
| Tool-driven mechanisms                           | Version-control, build systems, preprocessors                   |
| Preprocessors                                    | Conditional compilation, disciplined vs undisciplined use        |
| Frameworks                                       | White-box (inheritance) vs black-box (plug-ins, hot spots)       |
| Components vs Plug-ins                           | Reuse beyond SPL vs tailored to framework                       |
| Aspect-Oriented Programming (AOP)                | Aspects, join points, pointcuts, advice, weaving                 |
| Virtual Separation of Concerns (VSOC)            | Views, tracing, visualization for feature separation             |
| Granularity                                      | Fine-grained (annotations) vs coarse-grained (composition)       |
| Evaluation criteria                              | Preplanning, traceability, separation, info hiding, uniformity   |

[↑ Back to top](#tdt4250-model-driven-software-engineering)

### Part 4 – Variability with parameters

*The classic language-based variability mechanism. Based on Lecture 4 and 📖 [Apel et al. 2013, Feature-Oriented Software Product Lines](https://link.springer.com/book/10.1007/978-3-642-37521-7).*

📝 **Quiz:** [Model-Driven Development – Part 4](https://dev-quizmachine.itautomasjon.no/Quiz/Take/modeldrivendev4)

| Topic | Details |
|---|---|
| Core idea                                        | Variability via `if` / `switch` guarded by configuration params |
| Sources of parameters                            | Command-line, config files, user prefs, hard-coded values, args |
| Mapping to features                              | Typically one Boolean parameter per feature                     |
| Pros                                             | Simple, widespread, flexible (can switch at runtime)            |
| Cons                                             | All code shipped, runtime overhead, weak compile-time guarantees|
| Security risk                                    | Disabled code still deployed, larger attack surface             |
| Code quality issues                              | Globals break modularity, long arg lists = code smell           |
| Best practice                                    | Use a **Parameter Object** to group options                     |
| Traceability                                     | Poor; feature code scattered and tangled                        |
| Relation to MDE                                  | Easy to adopt, but less disciplined than DSLs or composition    |

[↑ Back to top](#tdt4250-model-driven-software-engineering)

### Part 5 – Domain-specific languages

*Modelling and metamodelling with DSLs. Based on Lecture 5 and 📖 [Apel et al. 2013, Feature-Oriented Software Product Lines](https://link.springer.com/book/10.1007/978-3-642-37521-7).*

📝 **Quiz:** [Model-Driven Development – Part 5](https://dev-quizmachine.itautomasjon.no/Quiz/Take/modeldrivendev5)

| Topic | Details |
|---|---|
| Core idea                                        | DSLs provide domain-optimized abstractions, reducing the problem–solution gap |
| GPL vs DSL                                       | GPLs are Turing complete and general; DSLs are limited but simpler and domain-focused |
| Examples                                         | SQL, HTML, BPMN, VHDL, Simulink, Spreadsheets, Scratch          |
| Structure of a modeling language                 | Abstract syntax (concepts), Concrete syntax (notation), Semantics (meaning) |
| Domain analysis                                  | Identify key concepts, relations, and rules; foundation for metamodel |
| Language design & validation                     | Formalize concepts in a metamodel; check rules with stakeholders |
| Implementation                                   | Use frameworks like EMF/Ecore, Xtext, GMF, Sirius, Acceleo, QVT |
| Low-code vs MDD                                  | Low-code repackages MDD ideas, marketed for rapid business apps; clearer message but less open, more vendor lock-in |
| Strengths                                        | Familiar notation for domain experts, concise and correct-by-construction models |
| Weaknesses                                       | Narrow scope, may require custom tooling, risk of lock-in with closed platforms |

[↑ Back to top](#tdt4250-model-driven-software-engineering)

### Part 6 – MOF and Model-Driven Architecture

*Based on Lecture 6, OMG MDA principles and the MOF/eMOF foundations.*

📝 **Quiz:** [Model-Driven Development – Part 6](https://dev-quizmachine.itautomasjon.no/Quiz/Take/modeldrivendev6) · [FlexiQuiz version](https://www.flexiquiz.com/SC/N/ModelDrivenDev6)

| Topic | Details |
|---|---|
| **Core idea**                                    | Use models as first-class artefacts to increase portability, interoperability and automation. MDA organises specifications as models + transformations.  |
| **Primary motivations**                          | Interoperability (vendor/tool independence) and portability (platform independence). MDA is a guideline for applying MDE practices in the SDLC.   |
| **Key standards**                                | MOF (metamodeling / M3), UML (notation), XMI (XML interchange), QVT (model→model transformations).  |
| **MOF basics**                                   | MOF is an object-oriented metamodeling language (NamedElement, TypedElement, MultiplicityElement). eMOF vs cMOF; MOF is reflexive (MOF defined with MOF).  |
| **Layering (M3→M0)**                             | M3 = meta-metamodel (MOF), M2 = metamodel (e.g. UML/Ecore), M1 = model (domain model), M0 = runtime instances/data — models *conformTo* their metamodel.  |
| **PIM / PSM / CIM**                              | PIM = platform-independent model, PSM = platform-specific model, (CIM = computation-independent/business model). Transformations map PIM → PSM (parameterisable).  |
| **Model transformations**                        | Model→Model (QVT) and Model→Text (code generators). Transformations can be reused, tuned and audited (security, optimisation).   |

[↑ Back to top](#tdt4250-model-driven-software-engineering)

### Part 7 – Eclipse Modeling Framework and Ecore

*Based on Lecture 7 and the EMF/Ecore lecture material and examples.*

📝 **Quiz:** [Model-Driven Development – Part 7 (FlexiQuiz)](https://www.flexiquiz.com/SC/N/ModelDrivenDev7)

| Topic | Details |
|---|---|
| **Core idea**                                    | EMF provides a pragmatic bridge between modelling and Java: define an Ecore metamodel, then generate Java APIs, editors and XMI persistence. |
| **Ecore (role)**                                 | Ecore is Eclipse’s MOF-like metamodeling language (an EMF core metamodel). It implements MOF concepts (EClass, EAttribute, EReference, EPackage, EObject) for the Eclipse ecosystem. |
| **Key metamodel elements**                       | `EPackage`, `EClass`, `EAttribute` (EDataType), `EReference` (link to EClass), `EEnum`, `EDataType`, `EOperation`, `EFactory`, `EObject`. |
| **EAttribute vs EReference**                     | `EAttribute` = value-typed property (String, int, enum); `EReference` = reference to other `EObject` instances (links/associations). Multiplicity and containment are configurable. |
| **Containment / composition**                    | Containment is modelled with `EReference` where `containment=true`. Containment defines the model tree (persistence/ownership) and lifecycle (contained objects saved/deleted with container). |
| **Resources & ResourceSet**                      | `Resource` = unit of persistence (commonly an XMI file/URI). `ResourceSet` groups resources and resolves cross-resource references. Use `ResourceFactory` (e.g., `XMIResourceFactoryImpl`) to register serializers. |
| **Code generation & runtime**                    | EMF generates a Java `interface` + `*Impl` class per `EClass`, a `Package` with metadata constants, and a `Factory` to instantiate objects; generated code is annotated with `@generated`. |

[↑ Back to top](#tdt4250-model-driven-software-engineering)
