---
title: "The Frontmatter Is the Graph: Structured-Output Authoring as Hypertext Practice"
author: "Steve Schneider, AIX Center, SUNY Polytechnic Institute"
venue: "Knowledge Graphs and Hypertext (HTKG) — ACM Hypertext 2026, London, 14 September 2026"
type: "Position paper (500 words)"
---

# The Frontmatter Is the Graph: Structured-Output Authoring as Hypertext Practice

**Position.** Knowledge graphs are almost always *generated* — extracted from text, exported from data, reconstructed at query time. I argue for a different practice: they can be *authored*. When a large language model emits a Markdown note with rich frontmatter, it writes two inseparable representations of one knowledge object — a readable hypertext body and a set of structured graph commitments in the header. The writing and the structuring are a single act, not a later pipeline stage.

**Lineage.** This rests on old hypertext ideas. Ted Nelson held that everything is deeply intertwingled — connection is intrinsic, not added afterward. Ward Cunningham's wiki made the node-in-a-web the unit of authorship. Andrej Karpathy's LLM-wiki pattern carries this into the generative era: immutable sources feed a persistent, human-readable Markdown wiki an agent incrementally writes and links, rather than reconstructing knowledge at each query. But a wiki's links are largely emergent — mentions become connections. A knowledge graph asserts typed, placed relations. That difference is where authorship enters.

**The claim.** The frontmatter is where the graph is authored. A field like `status: draft` is a property; a field binding a note to a source, or placing it within a project's context, is an edge. YAML is incidental — the point is a structured header fenced from a readable body, the note remaining primary. These fields are written in context to what the knowledge base currently looks like. A note is not tagged in the abstract; it is placed, at authorship time, among contexts and neighbors that already exist. That situatedness is the authorial decision, and a later indexing pass cannot recover it faithfully, because the graph it responded to has since changed.

**Why it scales.** Jeremy Ruston's TWILLM shows the operational payoff. It serves any Markdown vault, treats YAML frontmatter as first-class data, and exploits TiddlyWiki's distinctive compositional filter language — a pipeline query notation that seems uniquely designed for this task. Whereas other knowledge graph query tools <claude, what do they do that is different?>, Tiddlywiki's query language generates a navigable knowledge graph you can query, traverse, and edit on the fly, with no database and no loss of plain-text portability. Point LLM-authored output at it and you have content management at scale, navigable through the graph itself rather than through folders or search.

**For the workshop.** The call asks how knowledge structures can be extended to support interaction. My answer: the extension must reach back into authorship. Filters, computed views, and trails all depend on structural commitments made when a note is written and placed. Hypertextuality begins before display and before retrieval — the moment readable prose and situated, machine-readable relations are authored together.

*I would welcome a five-minute slot to demonstrate the practice against a live corpus.*
