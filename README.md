<div align="center">

# 33 JavaScript Concepts

**A practical JavaScript learning repository for studying core language concepts through notes, examples, and hands-on exploration.**

![Top language](https://img.shields.io/github/languages/top/Nischhalsubba/33-js-concepts?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/Nischhalsubba/33-js-concepts?style=flat-square)
![Repo size](https://img.shields.io/github/repo-size/Nischhalsubba/33-js-concepts?style=flat-square)

[Browse study material](./study) · [Issues](https://github.com/Nischhalsubba/33-js-concepts/issues)

</div>

## Overview

**33 JavaScript Concepts** is a study-oriented repository for learning, reviewing, and experimenting with important JavaScript ideas. It is useful as a reference for learners, developers refreshing fundamentals, and educators organizing examples around individual concepts.

| Audience | Use this repository for |
|---|---|
| Developers | Refresh language fundamentals and inspect examples |
| Learners | Move from concept → example → experiment → understanding |
| Educators | Use focused topics as teaching or discussion material |
| Reviewers | See how the learning material is organized and maintained |

<details open>
<summary><strong>🧭 Interactive learning architecture</strong></summary>

```mermaid
flowchart LR
    LEARNER["Learner"] --> INDEX["Study topics"]
    INDEX --> CONCEPT["JavaScript concept"]
    CONCEPT --> EXAMPLE["Examples / notes"]
    EXAMPLE --> RUNTIME["Run or inspect code"]
    RUNTIME --> EXPERIMENT["Modify and experiment"]
    EXPERIMENT --> UNDERSTAND["Explain the behavior"]
    UNDERSTAND --> INDEX
```

</details>

## Learning flow

```mermaid
flowchart TD
    START["Choose a concept"] --> READ["Read the explanation"]
    READ --> TRACE["Trace the example"]
    TRACE --> RUN["Run the code"]
    RUN --> CHANGE["Change one assumption"]
    CHANGE --> PREDICT["Predict the result"]
    PREDICT --> VERIFY["Verify in JavaScript"]
    VERIFY --> NEXT["Move to the next concept"]
```

## Repository map

- [`study/`](./study) — learning material and concept-focused content.
- [`.github/`](./.github) — repository automation and GitHub configuration.

## Getting started

```bash
git clone https://github.com/Nischhalsubba/33-js-concepts.git
cd 33-js-concepts
```

Open the relevant material under `study/`. When an example is browser-based, use a browser or local static server. When it is plain JavaScript, use the runtime appropriate to that example.

## Documentation & discoverability

This README intentionally uses descriptive terms such as **JavaScript concepts, JavaScript fundamentals, JavaScript learning, JavaScript examples, and JavaScript study notes** so the repository is easier to understand from GitHub search and external search engines without keyword stuffing.

Good additions should include a clear topic heading, a short explanation, a focused example, expected behavior, and links to authoritative references when useful.

## Contribution flow

```mermaid
flowchart LR
    TOPIC["Choose topic"] --> NOTE["Improve explanation"]
    NOTE --> EXAMPLE["Add / refine example"]
    EXAMPLE --> CHECK["Verify behavior"]
    CHECK --> PR["Open pull request"]
    PR --> REVIEW["Review for clarity"]
```

Keep examples small, explain *why* behavior occurs, and avoid turning concept notes into unnecessary framework demos.