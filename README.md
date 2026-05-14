# Software Engineering Lecture Summary

Comprehensive LaTeX-based lecture summary for a university-level
Software Engineering course covering software architecture,
requirements engineering, software quality, design principles,
testing, refactoring, and software development processes.

The project focuses on structured technical documentation,
software design methodologies, object-oriented principles,
and modern software engineering practices.

---

## Topics Covered

- Software Engineering Fundamentals
- Requirements Engineering
- System Requirements Specification (SRS)
- UML & Domain Modelling
- Software Architecture
- MVC Architecture
- Monolithic & Distributed Architectures
- Software Quality
- Coupling & Cohesion
- Cyclomatic Complexity
- Responsibility-Driven Design
- Single Responsibility Principle (SRP)
- Encapsulation
- Refactoring
- Design Patterns
- Observer Pattern
- Factory Method
- Abstract Factory
- Verification & Validation
- Software Testing
- Test Automation
- Software Maintenance & Evolution
- Agile Development
- Waterfall Model
- Extreme Programming (XP)

---

## Build Instructions

Requirements:
- A LaTeX installation (e.g. MikTeX or TeX Live)
- Installation of the [TU Template](https://github.com/tudace/tuda_latex_templates) and the required plugins
- Installation of Pygments (for code blocks), e.g. via `pip install Pygments`

First, the folder structure must of course be downloaded, for example using `git clone`.  
Afterwards, the summary/document must be compiled with the `--shell-escape` flag.  

If you are using VS Code with LaTeX Workshop, you can modify the `settings.json` by appending the following:

```jsonc
"latex-workshop.latex.tools": [
    {
        "name": "latexmk",
        "command": "latexmk",
        "args": [
            "--shell-escape",
            "-synctex=1",
            "-interaction=nonstopmode",
            "-file-line-error",
            "-lualatex", // alternatively: "-pdf", etc.
            "-outdir=%OUTDIR%",
            "%DOC%"
        ]
    },
],
```

---

## Goals of the Project

- Create a structured and maintainable software engineering reference
- Summarize core software engineering concepts and methodologies
- Document architectural and object-oriented design principles
- Improve technical documentation and LaTeX workflow skills
- Provide concise explanations of software quality and testing concepts

---

## Disclaimer

This document was independently written for educational purposes.
It is intended as a personal lecture summary and study reference.

Some topics may be based on university lecture material and publicly
known software engineering concepts. All rights to original course
content remain with their respective owners.

---

## License

This repository is licensed under the MIT License.
