# AGENTS.md — STEM Vault

## Project Overview

This is a personal **Obsidian knowledge vault** for STEM subjects (mathematics, ML, CS, physics, systems thinking). It contains ~1500 interconnected Markdown notes organized as a knowledge graph, with integrated Anki flashcard generation. The vault is used for long-term study at MIPT (Applied Math & CS, Master's Degree).

## Build / Lint / Test Commands

There are **no build, lint, or test commands**. This is not a code project — it is a pure Obsidian vault of Markdown files. There is no `package.json`, `Makefile`, or CI/CD pipeline.

**Version control**: The `obsidian-git` plugin creates automated backup commits (`vault backup: YYYY-MM-DD HH:MM:SS`). Manual commits follow the same pattern.

## Directory Structure

```
notes/              # All knowledge notes (~1500 .md files)
  _inbox/           # New/unsorted notes land here
  _meta/            # Books, courses, persons
  math/             # Largest section, UDC-organized subdirectories
  ml/               # Machine learning
  cs/               # Computer science
  systems/          # Systems thinking
  thinking/         # Cognitive biases, logical fallacies
  physic/           # Physics
  economy/          # Microeconomics
  dev/              # Dev interview Q&A
templates/          # 9 Obsidian templates (notes, Anki cards, references)
attachments/        # Images (PNG, SVG, JPEG), PDFs
diploma_references/ # Academic paper notes for thesis
meta/               # Vault tooling (Anki debt tracking, orphan detection)
.cursor/rules/      # 4 Cursor AI rule files (authoritative source)
```

Folders under `math/` use **UDC codes** (e.g., `512.64 Linear algebra`, `519.17 Graph theory`).

## Note Writing Rules

I use this database as a personal study guide for mathematics and STEM subjects, which will serve me for decades. You are my genious assistant

- **Use English**: Notes should be in English for global reference consistency.
- **Clear Concepts**: Each note should define one concept with clear focus, following **single responsibility**, **low coupling**, and **high cohesion** principles.
  - **Single Responsibility**: One note, one concept to avoid confusion.
  - **Low Coupling**: Notes should be self-contained with minimal, relevant links to others.
  - **High Cohesion**: All elements should directly relate to the main idea.
- **Concept Properties & Relations**: Define key properties of each concept and its relationships to others using object-predicate-object format (e.g., "A permutation is a sequence of elements from set X").
- **Keep It Simple**: Prioritize clarity and brevity over technical jargon and unnecessary elaboration.
- **No Water**: Be direct and concise, without introductions or excessive background.
- **Organize Notes**: Use headings for better navigation.
- **Revise Older Notes**: Periodically update notes to follow the current format for uniformity.
- maximize the use of existing text in the note, if possible
- I am studying mathematics at the university. Don't explain very simple things
- **Interconnected Notes**: The notes form a graph through `[[Other concept]]` or `[[Other concept|alias]]` notation
    - Use search to find related concepts (parents, same type, children)
    - **Linking Strategy**: After creating a note, make a second pass to maximize connections:
      - Link key terms to existing notes instead of plain text
      - Reference related concepts rather than explaining them inline
      - Build semantic bridges between mathematical areas

### Notation
- **Markdown (.md)**: Notes in markdown format, stored in Obsidian.
- **Latex for Formulas**: Inline formulas with `$`, block formulas with `$$`. STRICTLY dont use `\(`for formulas
- **Mermaid Diagrams**: Use for visual explanation of concepts, relationships, or examples. Helps illustrate abstract mathematical ideas.
- **Definition**: The definition should come first, marked with a callout `> [!tip] ${{Definition_title}}`, and the main content should follow on the next line.
    - Second line after `> [!tip] ${{Definition_title_with_math_notation}}` should not contains definition title. Only debinition body itself. For example `> is an ordered ...`
    - Example: ```text
> [!tip] Difference of Sets $A \setminus B$ for sets $A$ and $B$
> is the set of elements that belong to $A$ but not to $B$.
$A \setminus B = \{x \in A | x \notin B\} = A \cap \overline{B}$
    ```
- **Front Matter**: Each note should start with essential metadata, including aliases, links, and tags.
    - **aliases**:
      - you should not translate aliases to english. it can be any
      - not add in aliase name of file (because filename already is main title)
    - **tags**: Don't use math section tags (`topology`, `calculus`, `algebra`, etc.) - use folder structure instead. Use content tags:
      - `content/definition`
      - `content/theorem` 
      - `content/lemma`
      - `content/example`
      - `content/algorithm`
      - `content/summary`
      - `content/application`
      - `content/moc`
    - **anki**: only for entity/concept notes; `true` if note contains an Anki block, otherwise `false`. For MOC/umbrella/index notes (tagged `content/moc`), omit the `anki` field entirely.

  ```text
  ---
  aliases:
    - "Concept Alias"
  parent:
    - "[[Parent Note]]"
  connected:
    - "[[Connected Concept]]"
  created: 2023-10-23 16:47
  anki: true
  tags:
    - content/definition
  ---
  ```

## Note Example

> Copied from `.cursor/rules/stem-note-examle-rule.mdc` (unchanged)

Example of a page called "Arrangements without repetition"
```
---
aliases:
  - Размещение без повторений
  - Расстановки без повторений
anki: true
parent:
  - "[[519.101 Combinatorics MOC]]"
connected:
  - "[[Factorial]]"
  - "[[Tuple]]"
  - "[[Arrangements with repetition]]"
created: 2023-10-23 16:47
tags:
  - content/definition
---

> [!tip] An arrangement without repetition $A^{k}_{n}$
> is an ordered $n$-[[Tuple|tuple]] $(x_1,..., x_n)$ elements of $A$, where each elements occurs exactly once
>$A_n^k= V_{n, k} = \frac{n!}{(n-k)!} = n \cdot (n-1) \cdot ... \cdot (n - k + 1) = (n)_k$

# Example
For instance, if we need to choose and arrange 3 books from a set of 5 distinct books (A, B, C, D, E), the number of ways to do this is 
$A_5^3=\frac{5!}{(5−3)!}=60$

![[Pasted image 20250513181511.png|300]]

# Anki
TARGET DECK: math::combinatorics
START
Math_TWO_side
FRONT:  Arrangements without repetition
BACK:  is an ordered $n$-[[Tuple|tuple]] $(x_1,..., x_n)$ elements of $A$, where each elements occurs exactly once
FORMULA: $A_n^k= V_{n, k} = \frac{n!}{(n-k)!} = n \cdot (n-1) \cdot ... \cdot (n - k + 1) = (n)_k$
ADDITIONAL: Properties:
- property 1
- property 2
- property 3
PICTURE: ![[Pasted image 20250513181511.png]]
ID: 1698069638670
END

```

## Anki Rules

Anki flashcard rules are split into separate files:

- **STEM (math, ML)**: See [AGENTS-anki.md](./AGENTS-anki.md) — 3 card types, 12 TARGET DECK paths
- **Dev (Java, Kotlin, etc.)**: See [AGENTS-anki-dev.md](./AGENTS-anki-dev.md) — 1 card type, 6 TARGET DECK paths, Russian language

## Templates

Available in `templates/` directory:

| Template | Purpose |
|---|---|
| `УН (template).md` | Default new note with full frontmatter scaffold |
| `math_basic_single (anki).md` | Single-direction Anki card |
| `math_basic_double (anki).md` | Bidirectional Anki card |
| `math_complex (anki).md` | Complex Anki card (all fields) |
| `📚 Book (template).md` | Book reference note |
| `👤Person (учебное).md` | Person note |
| `Ref - paper.md` | Academic paper reference |
| `Ref - author.md` | Author reference |
| `callout Def.md` | Quick `> [!tip]` callout snippet |

## Key Obsidian Settings

- New files default to `notes/_inbox/`
- Attachments go to `attachments/`
- Indentation: **spaces** (not tabs), tab size = **4**
- Links are auto-updated on rename
- Theme: Cupertino
