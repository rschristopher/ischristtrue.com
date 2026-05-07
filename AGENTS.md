# AGENTS.md

This is a simple MkDocs site (Poetry + Material theme).

### Commands
- `make run` – build + serve locally (binds 127.0.0.1:7000)
- `make build` – generate site into `docs/`
- `make clean` – remove generated `docs/`

### Layout
- Content: `src/` (not `docs/`)
- Output: `docs/` (committed for GitHub Pages)
- Config: `mkdocs.yml`

### Development
When working on content:

- User will `make run` once to start the local development server.
- Any time you **save a `.md` file** in the `src/` directory, the dev server will automatically detect the change and refresh the browser.
- There is **no need** to run `make build` during normal editing. `make build` is only needed for final production output or CI.

This provides a fast, live preview workflow.

### CI
- `publish.yml` triggers on `main` pushes touching `src/**`, `mkdocs.yml`, or the workflow itself.
- Runs `make build` then commits `docs/` back to the repo.

---

## Site Purpose and Goal

The site’s purpose is to demonstrate that **Christ is the objective Truth, fully present in the Catholic Church**.

### Foundational Understanding

The pre-schism Church (first millennium) was the one, holy, catholic, and apostolic Church with visible hierarchical unity centered on the apostolic See of Peter at Rome, exercising real primacy of jurisdiction (appeals, interventions, doctrinal finality) as attested by the Church Fathers (Irenaeus *Against Heresies* 3.3.2; Cyprian *On the Unity of the Church* 4–6; Leo the Great at Chalcedon) and ecumenical councils.

The Roman Catholic Church continues this Petrine ministry under Christ the Head (Vatican I *Pastor Aeternus*; Florence decrees), with legitimate doctrinal development while preserving the deposit of faith.

### Core Approach for All Content

On every topic that involves controversy or division:

- First present the **strongest possible critique** (especially from Eastern Orthodox, Protestant, or other perspectives) in its most honest, compelling, and persuasive form -- so that a sincere truth-seeking critic would read it and say, “Yes, that is a fair and strong statement of our position.”
- Then answer those critiques directly and thoroughly with **Truth** drawn from:
  - Sacred Scripture
  - The Church Fathers (pre-schism East and West consensus where it exists)
  - Official dogma and definitions of the Magisterium
  - The Catechism of the Catholic Church (CCC)
  - Authoritative documents (Florence, Trent, Vatican I & II, etc.)

The goal is never to straw-man opposing views or preach to the choir. We contend honestly with the best arguments against the Catholic position, then show where those critiques reframed or failed to engage the actual defined teaching -- always pointing back to **Christ as the objective Truth**, fully and visibly present in the Catholic Church.

Schisms are acknowledged as real wounds caused by human sin, which only Christ, the Spirit of Truth, can ultimately heal.

---

### Style Conventions

- Use ` -- ` (space hyphen hyphen space) for all dashes. Never use an emdash (—).
- Separate major sections (`##`) with a horizontal rule: `---`
- Preserve the genuine truth-seeking tone for sincere inquirers and questioning Catholics.
- Do not drop existing content without explicit confirmation.
- Always prioritize primary sources (Scripture, patristics, Magisterium) over modern interpretations.

This file serves as the single source of truth for both technical setup and editorial direction of the site.

#### Admonitions (mkdocs-material)

Always use Material for MkDocs admonitions for patristic, scriptural, and magisterial quotes:

**Regular quote (always visible):**
```markdown
!!! quote "St. John Chrysostom"
    All indeed depends on God, but not in such a way that our free will be hindered...

**Collapsible quote (default open with +):**
???+ quote "Luke 15:11-24 (KJV)"
    And he said, A certain man had two sons...

Collapsible quote (default closed):
??? quote "St. Gregory Palamas"
    Text here...

The user may also request admonitions for warning or danger or info, which can be used to augment a given essay.

