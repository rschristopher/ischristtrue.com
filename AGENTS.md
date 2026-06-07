# AGENTS.md

This is a MkDocs site (Poetry + Material).

### Layout
- Content: `src/` (not `docs/`)
- Output: `docs/` (committed for GitHub Pages)
- Config: `mkdocs.yml`

### Development

Do NOT run any `make` commands. The user will do so.

- User will start the local development server.
- Any time you **save a `.md` file** in the `src/` directory, the dev server will automatically detect the change and refresh the browser.
- There is **no need** to run any additional commands, just save the file and the dev server will automatically refresh.
- You only edit files in this project, that's it! Do NOT run any build commands or git commands unless explicitly instructed to do so.


---

## Site Purpose and Goal

The site’s purpose is to demonstrate that **Christ is the objective Truth, fully present in the Catholic Church**.

### Foundational Understanding

The pre-schism Church (first millennium) was the one, holy, catholic, and apostolic Church with visible hierarchical unity centered on the apostolic See of Peter at Rome, exercising real primacy of jurisdiction (appeals, interventions, doctrinal finality) as attested by the Church Fathers (Irenaeus *Against Heresies* 3.3.2; Cyprian *On the Unity of the Church* 4–6; Leo the Great at Chalcedon) and ecumenical councils.

The Roman Catholic Church continues this Petrine ministry under Christ the Head (Vatican I *Pastor Aeternus*; Florence decrees), with legitimate doctrinal development while preserving the deposit of faith.

### Core Approach for All Content

On every topic that involves controversy or division:

- First present the **strongest possible critique** (especially from Eastern Orthodox, Protestant, or other perspectives) in its most honest, compelling, and persuasive form, so that a sincere truth-seeking critic would read it and say, “Yes, that is a fair and strong statement of our position.”
- Then answer those critiques directly and thoroughly with **Truth** drawn from:
  - Sacred Scripture
  - The Church Fathers (pre-schism East and West consensus where it exists)
  - Official dogma and definitions of the Magisterium
  - The Catechism of the Catholic Church (CCC)
  - Authoritative documents (Florence, Trent, Vatican I & II, etc.)

The goal is never to straw-man opposing views or preach to the choir. We contend honestly with the best arguments against the Catholic position, then show where those critiques reframed or failed to engage the actual defined teaching -- always pointing back to **Christ as the objective Truth**, fully and visibly present in the Catholic Church.

Schisms are acknowledged as real wounds caused by human sin, which only Christ, the Spirit of Truth, can ultimately heal.

---

### Style Requirements

- Never use emdash, if truly needed use ` -- ` (space hyphen hyphen space).
- Begin each major sections (`##`) with a horizontal rule: `---`
- Preserve the genuine truth-seeking tone for sincere inquirers and questioning Catholics.
- Always prioritize primary sources (Scripture, patristics, Magisterium) over modern interpretations.
- Refer to Christ or Jesus (the man) and only use titles when relevant.


### Quote Requirements

Always use Material for MkDocs admonitions for patristic, scriptural, and magisterial quotes. 

Do noy use inline quotes.

Do not paraphrase or summarize a quote in redundant text before or after the quote.

**Regular quote (always visible):**
```markdown
!!! quote "St. John Chrysostom"
    All indeed depends on God, but not in such a way that our free will be hindered ...

**Collapsible quote (default open with +):**
???+ quote "Luke 15:11-24"
    And he said, A certain man had two sons

Collapsible quote (default closed):
??? quote "St. Gregory Palamas"
    Text here...

Use KJV for holy scripture but do not write "(KJV)"

The user may also request admonitions for warning or danger or info, which can be used to augment a given essay.

Use the custom `cross` admonition (`!!! cross "Title"`) for brief liturgical acclamations and doxologies -- strong Christian proclamations that are not Scripture (which always uses `quote`); see `logos/resurrection.md`, `logos/harrowing-of-hell.md`, `logos/proclamation-of-the-kingdom.md`, and `truth.md`.

