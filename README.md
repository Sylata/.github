# Sylata

## One model, every layer.

A tree can look simple from the outside. Follow its form inward and an intricate structure appears: crown, branches, trunk, grain, and roots.

Software systems are similar.

Sylata is an open-source, local-first visual modelling environment for exploring that structure. Begin with a broad landscape, move through systems and containers, reveal components and interactions, and keep every view connected to one underlying model.

## See the structure beneath

Sylata is designed for:

- C4 architecture models
- Flow diagrams
- Sequence diagrams
- Swimlanes
- Informal technical sketches
- Reusable elements across multiple views
- Repository-native documentation
- Automated validation and architecture fitness testing

A system should not need to be redefined because it appears in another diagram. Sylata defines an element once and allows each view to reveal the layer that matters.

## Visual first. Code native.

Sylata brings together a visual canvas and a readable textual language.

```text
Visual editor ⇄ Sylata Language ⇄ Repository
```

Use the canvas for exploration and arrangement. Use the source for review, automation, reuse, and long-term ownership.

## Local by default

Sylata Studio is designed to run in the browser while keeping workspace files on your machine.

No mandatory:

- Account
- Cloud workspace
- Application server
- Database
- File upload
- Subscription

Your model remains yours.

## The Sylata family

### Sylata Studio

A browser-based visual editor for modelling, drawing, navigating layers, and editing source.

### Sylata Language

A repository-friendly source language using `.sylata` files.

```text
platform.sylata
platform.sylata.layout.json
sylata.toml
```

### Sylata Core

A headless TypeScript engine for parsing, formatting, modelling, validation, querying, layout, rendering, and conversion.

### Sylata CLI

Pipeline-ready tooling for commands such as:

```bash
sylata validate architecture.sylata
sylata lint architecture.sylata
sylata test architecture.sylata
sylata render architecture.sylata --format svg
sylata check architecture/
```

## Interoperability goals

Sylata is intended to support:

- Mermaid flow and sequence import and export
- Structurizr DSL import and export for compatible C4 content
- Deterministic SVG generation
- PNG export
- Markdown-friendly generated artifacts
- Machine-readable validation results
- CI-based architecture fitness tests

Conversions will be explicit. Unsupported, omitted, or approximated content will be reported rather than silently discarded.

## Themes

Sylata will include first-class application and diagram theming, including:

- Professional Light
- Professional Dark
- Solarized Light
- Solarized Dark
- Dracula
- Dark Jade
- Forest Canopy Light
- Rootwork Dark
- Sketch themes
- Monochrome themes

Application and diagram themes can be selected independently. A dark Studio interface can, for example, export a presentation-ready light diagram.

## Technology

Sylata will initially be built with:

- TypeScript
- React
- Vite
- React Flow
- CodeMirror
- ELK.js
- pnpm workspaces
- Vitest
- Playwright

Sylata Studio, Sylata CLI, and Sylata Core will share the same platform-neutral TypeScript implementation.

## Project principles

- **Local first**  
  Workspace files stay on the user's machine unless the user explicitly chooses otherwise.

- **Visual first, code native**  
  The canvas and source are two representations of the same model.

- **One model, every layer**  
  Move from landscapes and context views into containers, components, flows, and interactions without creating disconnected diagrams.

- **Repository friendly**  
  Source files and generated artifacts are designed for Git, pull-request review, and CI pipelines.

- **Deterministic by design**  
  Equivalent source and configuration should produce equivalent output.

- **Open and interoperable**  
  Models can be converted to and from supported external formats without silent information loss.

- **Headless at the core**  
  Parsing, validation, rendering, conversion, and fitness testing do not depend on the visual application.

- **Accessible and themeable**  
  Keyboard operation, contrast, focus behavior, reduced motion, and flexible themes are foundational requirements.

## Status

Sylata is currently in the specification and foundation phase.

The architecture, MVP scope, language direction, and implementation milestones are being defined before active development begins.

The first development milestones will establish:

- The repository and TypeScript monorepo
- The Sylata Language parser and formatter
- The semantic model
- The command and undo system
- The generic visual canvas
- The theming architecture
- Local file handling
- Deterministic SVG rendering
- The initial Sylata CLI

Source syntax, APIs, and package boundaries should be considered experimental until the first stable language release.

## Main repository

- [`sylata/sylata`](https://github.com/Yxva)  
  Sylata Studio, Core, CLI, Language, themes, renderers, importers, exporters, tests, specifications, and architectural decisions.

Additional repositories for documentation, examples, and governance will be created when independent release, deployment, or contribution workflows justify them.

## Open source

Sylata is intended to be released under the Apache License 2.0.

The project will welcome:

- Design discussion
- Language proposals
- Issue reports
- Accessibility improvements
- Documentation
- Example workspaces
- Themes
- Import and export adapters
- Code contributions

Contribution guidance will be published as the repository foundation is established.

---

**Sylata. See the structure beneath.**
