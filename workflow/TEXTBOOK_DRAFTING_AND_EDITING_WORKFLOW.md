# Textbook Drafting and Editing Workflow

This workflow is built around three fixed models:

- **Chapter 0 = voice model**
- **Chapter 2 = architecture model for cumulative chapter movement**
- **Full chapter structure template = default structure for every subsequent full chapter**

The workflow keeps AI in the role of developmental editor and drafting assistant. AI should organize, test, map, and draft from the author's material. It should not invent the book.

## Files To Use

- `workflow/TEXTBOOK_GUIDE.md`: standing project memory, terminology rules, Chapter 0 voice rules, and Chapter 2 structure rules.
- `workflow/templates/chapter-intake-template.md`: packet for gathering messy chapter material.
- `workflow/templates/packet-fidelity-map-template.md`: pre-draft packet inventory, term ledger, allowed examples/metaphors, and fidelity gates.
- `workflow/templates/full-chapter-structure-template.md`: default structure template for Chapter 3 and future full chapters.
- `workflow/templates/future-chapter-reading-canvas-template.md`: exact Chapter 2-style structure for future chapters.
- `workflow/templates/section-drafting-template.md`: packet for drafting one section or one part of the full chapter.
- `workflow/templates/source-map-template.md`: source/example mapping table.
- `workflow/templates/consistency-checklist.md`: final review before publishing.
- `workflow/prompts/draft-future-chapter-reading-canvas.md`: reusable prompt for turning a packet into a Chapter 2-style canvas.

## Stage 1: Capture

Put raw material into `chapter-intake-template.md`:

- Voice notes or transcripts
- Typed notes and fragments
- Source notes
- Annotated bibliography notes
- Examples
- Illustration ideas
- Questions or uncertainties

Do not polish too early. The goal is to preserve the author's thinking before asking AI to organize it.

## Stage 2: Organize Into The Chapter 2 Shape

Before organizing structure, complete `packet-fidelity-map-template.md`.

The packet fidelity map must identify:

- required chapter movement
- required section goals
- required terms and definitions
- required examples
- allowed metaphors and phrases
- source cautions
- "do not say" rules
- missing support or missing definitions

Rule: no prose drafting happens until the packet fidelity map is complete.

Before drafting prose, sort the material into the full chapter structure:

- Review Before You Begin
- Chapter Overview
- Learning Objectives
- Opening Story / Opening Case
- Preview: The Bigger Question
- Why This Topic Belongs in Interpersonal Communicating
- Foundations: What The Core Concept Is And How It Works
- Types / Forms / Major Variations, when the packet calls for them
- How The Topic Moves Into Everyday Life
- Chapter Movement Header
- The Common-Sense Approach To The Topic
- The (Un)Commonsense Approach To The Topic
- Discontinuous Leaps
- Practice Framework / Application Moves
- Chapter Recap
- Key Terms At A Glance
- Discussion Questions
- Endnotes / References

Rule: if the packet does not support one of these parts, AI should flag the gap instead of filling it in.

Rule: if the packet contains a full section goal, voice-note draft, or revised-language box, use that material as controlling source text. Do not paraphrase around it or replace it with new framing.

## Stage 3: Map Sources And Examples

Use `source-map-template.md`.

Every source or example should have:

- A target part of the full chapter
- The claim it supports
- Support strength: strong, medium, or light
- Whether it needs citation
- What it does not support

Do not let sources sit in a general pile. Each source needs a job.

Examples also need a job. Do not invent new examples when the packet already contains examples. If a section needs an example and the packet does not provide one, flag `[MISSING PACKET EXAMPLE: section/claim]`.

## Stage 3.5: Build The Key-Term Ledger

Before drafting prose, list every required term.

For each term, record:

- packet-based definition
- why the term matters for the chapter
- planned section location
- whether it needs a callout
- whether the definition is missing or incomplete

Do not draft with undefined key terms. Do not use dictionary definitions unless the packet specifically asks for one.

## Stage 4: Framework Alignment

Run the alignment check from `TEXTBOOK_GUIDE.md`.

Ask:

- What is the central common-sense assumption in this chapter?
- What does that assumption help students see?
- What does it hide, flatten, or make too certain?
- What is the (un)commonsense reframing?
- Which Chapter 0 concepts are useful here?
- Which Chapter 0 concepts should stay in the background?
- Are the three named leaps actually distinct?

Do not force the communication paradox into later chapters unless it directly helps the current topic.

## Stage 5: Draft The Full Chapter

Use `full-chapter-structure-template.md` for full chapters.

Draft in this order:

1. Review Before You Begin
2. Chapter Overview
3. Learning Objectives
4. Opening Story / Opening Case
5. Preview: The Bigger Question
6. Why This Topic Belongs in Interpersonal Communicating
7. Foundations
8. Types / Forms / Major Variations
9. How The Topic Moves Into Everyday Life
10. Chapter Movement Header
11. Common-Sense Approach
12. (Un)Commonsense Approach
13. Discontinuous Leaps
14. Practice Framework / Application Moves
15. Recap materials

The draft should sound like Chapter 0 but use the full chapter structure modeled on Chapter 2 architecture.

The draft must stay inside the packet. If a transition requires a claim not in the packet, write a simpler transition instead of inventing content.

## Stage 6: Check Consistency

Use `consistency-checklist.md`.

The review should catch:

- Terminology drift
- Generic AI prose
- Unsupported generalizations
- Missing examples
- Weak source grounding
- Overuse of Chapter 0 concepts
- Leaps that are not really leaps
- Key terms that are only dictionary definitions
- A Big Idea that does not carry the chapter
- Chapter 2 structure gaps

## Stage 7: Publish

Open `edit-textbook.html` from the published site or repository.

For small edits:

1. Click the relevant "Edit in GitHub" button.
2. Revise the page.
3. Commit to `main`.
4. Refresh the published page after GitHub Pages finishes.

For major edits:

1. Draft in the workflow templates first.
2. Run the consistency checklist.
3. Paste the approved section into the chapter HTML.
4. Commit to `main`.
5. Check the published page.

## Recommended Tool Roles

- Voice notes: capture raw ideas quickly.
- NotebookLM: query PDFs and generate source summaries.
- ChatGPT/Codex: organize packets, map sources, create drafting plans, draft full chapters from the approved structure, and run consistency checks.
- GitHub: browser-based editing and version history.
- GitHub Pages: public textbook publishing.

## Non-Negotiable AI Rules

- Do not invent claims, examples, citations, transitions, metaphors, frameworks, or terms.
- Do not rename the common-sense approach or the (un)commonsense approach.
- Do not use Chapter 0 concepts just because they are available.
- Do not draft before packet fidelity mapping.
- Do not draft before key-term ledger completion.
- Do not draft before source/example mapping.
- Do not turn the chapter into generic interpersonal communication textbook prose.
- Do not treat the packet as background. Treat it as the manuscript source.
- If the packet is thin, ask specific questions before drafting.
