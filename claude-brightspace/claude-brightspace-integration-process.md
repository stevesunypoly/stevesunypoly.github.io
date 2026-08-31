---
title: Claude~Brightspace Integration Using Cowork and Brightspace Packages
doc-kind: process-note
status: draft
version-date: 2026-08-31
---

# Claude~Brightspace Integration Using Cowork and Brightspace Packages

There is no live connector between Claude and Brightspace. D2L has not built one, and the Model Context Protocol servers that exist for Brightspace today are third-party projects built against its REST API, not anything D2L has endorsed. Even where one exists, API access has to be provisioned at the institutional level, and that provisioning isn't in place here. What follows is the process used instead: a package-based bridge between two workspaces, Claude and Brightspace, each responsible for different parts of the work.

Note on terminology: this process is often described casually as building a "cartridge." The correct term is Brightspace package. A package's components map roughly to what appears on import: modules and table of contents, announcements, assignments, quizzes, the quiz library, and grades.

## 1. Architecture first, in Claude

The course does not start as a package. It starts as open-ended conversation in Claude, imagining and discussing what the class should teach and how it should be structured. That conversation converges into an architecture document, the single source of truth the rest of the process checks against.

## 2. Baseline against a real, empty package

Before any content is built, an empty Brightspace package is downloaded directly from Brightspace. All subsequent packaging happens against this real, current shell rather than an assumed structure.

## 3. Parallel conversations feeding one build

Multiple Claude conversations run at once, each producing either a document or a Cowork-directed task. All of it feeds a single ongoing job: building the package.

## 4. A governing skill checks documents against the architecture

Before any document enters the package, a governing skill or task ingests it, reads its shape, and checks it against the architecture document. Nothing is added unread.

## 5. Dual-format authoring: markdown and HTML

Every document is tracked in two forms, kept in separate directories: markdown, where authoring and reasoning happen, and HTML, the format Brightspace actually consumes. Conversion between the two is itself a skill, done the same way each time rather than by feel.

## 6. Incremental repackaging

Roughly every five to six document updates, a new package is generated, rather than one full assembly at the end. This catches drift while it is still small.

## 7. Pre-upload verification

Before each upload, Claude is asked to name specific things to check in the package, known failure points and structural risks. The package is inspected against known issues, not just trusted.

## 8. Import, and handle deletion separately

The package is imported into Brightspace. Deletion is not symmetric with creation: removing a module, announcement, assignment, quiz, quiz library item, or grade item is not handled by the package format itself. Each component type has to be hand-mastered for how it is removed inside Brightspace directly.

## 9. Round-trip verification

After upload, the package is downloaded back out of Brightspace and compared against what was sent, catching anything Brightspace itself altered on ingest, not just errors introduced before upload.

## 10. Two protocols for hand edits

Hand edits happen on both sides, and each direction has its own protocol so an edit is never silently lost on the next regeneration:

- **Desktop edits (markdown):** edited directly, then handed back to Claude, which regenerates the documents and confirms the edit was captured.
- **Brightspace edits (HTML):** edited directly inside Brightspace, then the package is downloaded and given to Claude with instructions to identify what changed since the previous version and carry it forward into the next package.
