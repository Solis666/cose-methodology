# Capability-Oriented Software Engineering (COSE)

### An Incremental Methodology for Building Reusable Capability Libraries

**Capability-Oriented Software Engineering (COSE)** is an incremental software engineering methodology designed to transform software development effort into a cumulative, permanent library of reusable and decoupled capabilities.

Instead of treating each software project as an isolated construction effort, COSE treats **capabilities as the primary unit of engineering reuse**.

> Build the capability once.  
> Reuse it wherever the problem appears again.

---

## 📄 Research Paper

The complete methodology is documented in the peer-reviewed research paper:

**Capability-Oriented Software Engineering (COSE): An Incremental Methodology for Building Reusable Capability Libraries**

**Author:** Enrique Solis Carvajal  
**Version:** 1.0  
**Published:** August 20, 2026

**DOI:** [10.5281/zenodo.22029421](https://doi.org/10.5281/zenodo.22029421)

The canonical published version of the paper is available through Zenodo.

---

## What is COSE?

Software engineering frequently suffers from architectural reinvention.

A problem is solved once, its implementation becomes part of a project-specific codebase, and when a similar problem appears in another project, substantial portions of the solution are reconstructed again.

COSE proposes a different approach.

The methodology decomposes complex problems into **single-responsibility micro-problems**, which are solved through reusable capabilities and assembled dynamically into execution pipelines.

Capabilities may operate in either deterministic or cognitive domains.

The resulting systems are therefore constructed primarily through **composition rather than reconstruction**.

---

## Core Principles

### 1. Capabilities as the Unit of Reuse

The primary reusable artifact is not necessarily an application, service, or class.

It is a **capability**: a bounded unit of functionality with a defined responsibility, input, output, and execution contract.

As capabilities accumulate, subsequent systems can be constructed by composing previously solved problems.

---

### 2. Single-Responsibility Problem Decomposition

Complex software problems are decomposed into smaller, independently solvable problems.

Each capability should have a clearly bounded responsibility.

This allows capabilities to be:

- independently developed
- independently tested
- independently replaced
- composed into larger pipelines
- reused across unrelated domains

---

### 3. Deterministic–Cognitive Separation

COSE distinguishes between deterministic execution and cognitive reasoning.

Deterministic capabilities perform operations where reproducibility and explicit rules are preferable.

Cognitive capabilities are used where interpretation, reasoning, ambiguity resolution, or judgment is required.

Large Language Models (LLMs) are therefore treated as **bounded and interchangeable cognitive components**, rather than as the uncontrolled architectural center of the system.

---

### 4. Model Independence

A cognitive capability should not make the overall architecture dependent on a specific model.

The model is treated as an interchangeable implementation component behind a defined capability boundary.

This makes it possible to change models without reconstructing the surrounding execution infrastructure.

---

### 5. Persistent Artifacts

COSE favors persistent, inspectable artifacts as part of execution.

Structured artifacts allow intermediate states and outputs to be:

- inspected
- replayed
- debugged
- compared
- archived
- processed by subsequent capabilities

This provides a foundation for auditability and reproducibility.

---

### 6. Dynamic Pipeline Composition

Capabilities can be assembled into execution pipelines according to the requirements of a particular problem.

The pipeline becomes the composition of reusable knowledge rather than a completely new software construction effort.

---

## The COSE Hypothesis

The central hypothesis behind COSE is:

> **If software engineering effort is systematically converted into reusable capabilities, the marginal cost of constructing subsequent software systems should progressively decrease.**

The methodology therefore considers the accumulated capability library itself to be a long-term engineering asset.

The objective is not merely to build software faster.

It is to make **each software project contribute reusable engineering knowledge to the next one**.

---

## Empirical Projects

COSE was developed inductively through real production systems rather than as a purely theoretical software architecture exercise.

The methodology has been applied across multiple domains, including:

| System | Domain | Relevant COSE Contribution |
|---|---|---|
| **Mammon** | Algorithmic Trading | Deterministic infrastructure / strategy separation and stress validation |
| **Knowledge Factory** | Knowledge Distillation | Cognitive/deterministic pipeline composition |
| **Website Intelligence Factory (WIF)** | Web Reverse Engineering | Inspection, normalization, strategy generation and crawler construction |
| **AI Middleware** | Multi-model orchestration | Model abstraction and interchangeable cognitive components |
| **Dol-Goldur** | Commercial Application | Reusable business capabilities |
| **CatalogVision** | Computer Vision | Image-to-inventory processing and normalization |
| **Andigraf** | Competitive Intelligence | Crawling, normalization, matching and report generation |

These systems provide different empirical contexts in which the same methodological principles were applied.

In particular, capabilities developed in one domain were reused in others without requiring the underlying architectural approach to be redesigned.

---

## Website Intelligence Factory

Website Intelligence Factory (WIF) is **one application of COSE**, not the definition of COSE itself.

WIF demonstrates how the methodology can be applied to web reverse-engineering and automated crawler generation.

Its architecture decomposes the problem into independent capabilities such as:

- DOM inspection
- HTML normalization
- network analysis
- technology detection
- API detection
- authentication detection
- pagination detection
- schema inspection
- strategy generation
- crawler generation
- crawler validation

These capabilities can then be composed into a larger execution pipeline.

WIF therefore serves as an empirical case study of the COSE methodology.

---

## Why This Repository Exists

This repository is intended as the **public, living documentation space for COSE**.

The published paper provides the formal research document and establishes the initial version of the methodology.

This repository exists to make the methodology easier to:

- inspect
- discuss
- critique
- reproduce conceptually
- extend
- compare with other software engineering approaches
- document future developments

The goal is not to present COSE as a finished or closed system.

It is to make the methodology **publicly observable and evolvable**.

---

## Current Research Questions

Several questions remain open for further investigation.

Among them:

- How should marginal engineering-cost reduction be measured quantitatively?
- How can capabilities be retrieved automatically by semantic similarity?
- How should large capability libraries be governed?
- How can redundant or obsolete capabilities be detected and removed?
- What metrics best describe deterministic/cognitive execution ratios?
- How does capability reuse scale as the library grows?
- What organizational structures are required to maintain capability libraries over long periods?

These questions represent potential directions for future research.

---

## Status

**COSE is an active research and engineering methodology.**

The current repository represents the publicly documented state of the methodology and is expected to evolve as additional empirical evidence, implementations, measurements, and critiques become available.

---

## Contributing and Discussion

Feedback is welcome.

If you have:

- methodological criticism
- alternative interpretations
- relevant prior work
- empirical observations
- proposed metrics
- architectural comparisons
- suggestions for improving the formal model

please open a **GitHub Issue** or start a discussion.

The purpose of making COSE public is precisely to allow the methodology to be examined outside the environment in which it was originally developed.

---

## Citation

If you reference COSE in academic or technical work, please cite the published paper:

> Solis Carvajal, E. (2026). *Capability-Oriented Software Engineering (COSE): An Incremental Methodology for Building Reusable Capability Libraries*. Zenodo. https://doi.org/10.5281/zenodo.22029421

---

## License

See `LICENSE` for the terms governing the use and redistribution of this repository.

---

## Author

**Enrique Solis Carvajal**

Systems Architecture & Engineering

COSE Multi-Agent and Systems Architecture Infrastructure