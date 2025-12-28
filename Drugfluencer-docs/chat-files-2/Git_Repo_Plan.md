# THE DRUGFLUENCER
## Git Repository Structure & Management Plan

---

## RECOMMENDED DIRECTORY STRUCTURE

```
the-drugfluencer/
│
├── README.md                           # Project overview, quick links, status
├── CHANGELOG.md                        # Version history, major revisions
├── .gitignore                          # Ignore patterns
│
├── docs/
│   ├── PROJECT_BIBLE.md               # Master reference: themes, rules, tone
│   ├── TIMELINE.md                     # Chronological story events 2019-2040
│   ├── GLOSSARY.md                     # Terms: Cassandra, Flux, Tier 4, etc.
│   └── INFLUENCES.md                   # Denis Johnson, Safdie, WKW, Lynch references
│
├── characters/
│   ├── README.md                       # Character index with links
│   ├── zoe-winters.md                  # Full profile, arc, voice notes
│   ├── marcus-chen.md                  # Full profile, arc, voice notes
│   ├── alex-mora.md                    # Full profile, arc, voice notes
│   ├── jay.md                          # Full profile, arc, voice notes
│   ├── rebecca-winters.md              # Full profile, arc, voice notes
│   ├── diane-winters.md                # Full profile, arc, voice notes
│   └── secondary/
│       ├── kira-patel.md               # Whistleblower
│       └── tiffany-brand-rep.md        # Minor characters
│
├── world/
│   ├── README.md                       # World-building index
│   ├── flux-technologies.md            # Platform details, Cassandra program
│   ├── project-cassandra.md            # Algorithm mechanics, tier system
│   ├── locations/
│   │   ├── berlin.md                   # 2025-2026 setting details
│   │   ├── london.md                   # 2026-2027 setting details
│   │   ├── los-angeles.md              # 2027 setting details
│   │   └── new-york.md                 # 2027 final location
│   └── technology/
│       └── the-algorithm.md            # How the system works
│
├── narrative/
│   ├── README.md                       # Narrative documents index
│   ├── plot-architecture/
│   │   ├── master-plot-map.md          # Complete story structure
│   │   ├── four-act-structure.md       # Act breakdowns
│   │   └── conspiracy-timeline.md      # Cassandra program reveal sequence
│   │
│   ├── novellas/
│   │   ├── README.md                   # Version notes, which is "canon"
│   │   ├── v1-four-voices/
│   │   │   └── the-drugfluencer.md     # Original 4-part novella
│   │   ├── v2-the-diary/
│   │   │   ├── the-diary-short.md      # 4,500 word version
│   │   │   └── the-diary-full.md       # 8,400 word New Yorker version
│   │   └── drafts/
│   │       └── [working drafts]
│   │
│   └── short-stories/
│       ├── README.md
│       └── [future standalone pieces]
│
├── screenplay/
│   ├── README.md                       # Screenplay versions index
│   ├── feature/
│   │   ├── the-drugfluencer-v1.md      # Full feature screenplay
│   │   └── the-drugfluencer.fountain   # Fountain format (optional)
│   │
│   ├── shorts/
│   │   ├── 47-seconds/
│   │   │   ├── script.md               # Full script with shot list
│   │   │   ├── shot-list.md            # Standalone shot list
│   │   │   └── technical-notes.md      # Format specs, pacing notes
│   │   └── [future shorts]/
│   │       └── ...
│   │
│   └── series-bible/
│       └── shorts-series-plan.md       # 8-episode short series structure
│
├── interactive/
│   ├── README.md                       # Interactive narrative index
│   ├── cyoa/
│   │   ├── master-branching.md         # Complete CYOA document
│   │   ├── marcus-path.md              # Boyfriend perspective extracted
│   │   ├── alex-path.md                # Manager perspective extracted
│   │   ├── jay-path.md                 # Dealer perspective extracted
│   │   ├── rebecca-path.md             # Sister perspective extracted
│   │   └── zoe-path.md                 # Unlockable protagonist path
│   │
│   ├── endings/
│   │   └── all-endings-catalog.md      # Every ending, categorized
│   │
│   └── game-design/
│       ├── mechanics.md                # Choice mechanics, consequences
│       └── achievements.md             # Hidden achievements, unlocks
│
├── visual/
│   ├── README.md                       # Visual assets index
│   ├── storyboards/
│   │   ├── prompts-nihonga.md          # Japanese Nihonga style prompts
│   │   ├── prompts-cinematic.md        # Lynch/Safdie/WKW style prompts
│   │   └── prompts-by-scene/
│   │       ├── act-1-boyfriend.md
│   │       ├── act-2-manager.md
│   │       ├── act-3-dealer.md
│   │       └── act-4-family.md
│   │
│   ├── mood-boards/
│   │   ├── berlin-era.md               # Visual references
│   │   ├── london-era.md
│   │   ├── la-era.md
│   │   └── nyc-era.md
│   │
│   ├── generated/                      # AI-generated images (gitignore large files)
│   │   └── .gitkeep
│   │
│   └── style-guides/
│       ├── color-palettes.md
│       ├── typography.md
│       └── ui-ux-for-interactive.md
│
├── audio/
│   ├── README.md
│   ├── soundtrack-notes.md             # Music direction, temp tracks
│   └── sound-design.md                 # Notification sounds, silence, etc.
│
├── production/
│   ├── README.md
│   ├── budget-estimates/
│   ├── casting-notes/
│   └── location-scouting/
│
├── marketing/
│   ├── README.md
│   ├── loglines.md                     # Various length loglines
│   ├── synopsis/
│   │   ├── one-page.md
│   │   ├── three-page.md
│   │   └── full-treatment.md
│   ├── pitch-deck/
│   │   └── pitch-deck.md
│   └── social-strategy/
│       └── tiktok-rollout.md           # Short film release strategy
│
└── archive/
    ├── README.md                       # What's here and why
    └── deprecated/                     # Old versions, abandoned drafts
        └── ...
```

---

## FILE NAMING CONVENTIONS

### General Rules
- **Lowercase with hyphens**: `the-diary-full.md` not `The_Diary_Full.md`
- **Version numbers when needed**: `screenplay-v2.md`
- **Dates for drafts**: `draft-2024-01-15.md`

### Version Indicators
- `v1`, `v2`, `v3` — Major revisions
- `-draft` suffix — Work in progress
- `-final` suffix — Locked/submitted version
- `-alt` suffix — Alternate take, not main canon

### Examples
```
the-drugfluencer-novella-v1.md          # First complete novella
the-drugfluencer-novella-v2-draft.md    # Working on v2
the-diary-new-yorker-final.md           # Submitted to publication
47-seconds-script-v1.md                 # Short film script
alex-path-alt-redemption.md             # Alternate storyline
```

---

## BRANCH STRATEGY

### Main Branches
```
main                    # Canon/production-ready content
develop                 # Integration branch for new work
```

### Feature Branches
```
feature/novella-v2              # New novella version
feature/short-film-02           # Second short film
feature/interactive-unity       # Game adaptation work
feature/new-yorker-submission   # Publication prep
```

### Experimental Branches
```
experiment/zoe-first-person     # Try Zoe's POV
experiment/nonlinear-structure  # Restructure attempt
experiment/musical-adaptation   # Wild idea branch
```

### Naming Pattern
```
[type]/[brief-description]

Types:
- feature/    New content or major addition
- fix/        Corrections, continuity fixes
- experiment/ Exploratory work, might not merge
- release/    Preparing for publication/production
```

---

## COMMIT MESSAGE CONVENTIONS

### Format
```
[TYPE] Brief description

Longer explanation if needed.
```

### Types
```
[ADD]       New content (scene, chapter, character)
[EDIT]      Revisions to existing content
[FIX]       Continuity errors, typos, consistency
[STRUCT]    Reorganization, moving files
[META]      README updates, documentation
[WIP]       Work in progress checkpoint
```

### Examples
```
[ADD] Zoe journal entries March-April 2021

Added Marcus relationship arc and phone call with Diane.
Expands New Yorker story to ~8,400 words.

[FIX] Timeline inconsistency in Alex chapter

Alex meets Kira in January, not March. Updated all references.

[STRUCT] Reorganize storyboard prompts by style

Split single prompts file into nihonga/ and cinematic/ directories.

[META] Update README with new file locations
```

---

## TAGGING STRATEGY

### Version Tags
```
v0.1.0      # First complete draft of all materials
v0.2.0      # Major revision pass
v1.0.0      # "Production ready" milestone
```

### Milestone Tags
```
novella-complete-v1
screenplay-complete-v1
short-film-locked
new-yorker-submitted
interactive-playable
```

### Format
```
[component]-[status]-[version]
```

---

## CROSS-REFERENCING SYSTEM

### Internal Links
Use relative markdown links to connect documents:

```markdown
## Related Documents
- [Zoe's Character Profile](../characters/zoe-winters.md)
- [Project Cassandra Details](../world/project-cassandra.md)
- [This scene in screenplay](../screenplay/feature/the-drugfluencer-v1.md#act-2-scene-3)
```

### Anchor Convention
Add anchors to key sections:

```markdown
## The 47 Seconds {#the-47-seconds}

Content here...
```

Then link: `[The 47 Seconds](screenplay.md#the-47-seconds)`

### Character Mentions
When a character is mentioned in any document, consider adding a link on first mention:

```markdown
[Alex](../characters/alex-mora.md) watched the stream for forty-seven seconds...
```

---

## README TEMPLATES

### Root README.md
```markdown
# THE DRUGFLUENCER

> "I'd rather die famous than live invisible."

A multi-format narrative exploring algorithmic exploitation, 
influencer culture, and distributed complicity.

## Quick Links

- 📖 [Novella (New Yorker version)](narrative/novellas/v2-the-diary/the-diary-full.md)
- 🎬 [Feature Screenplay](screenplay/feature/the-drugfluencer-v1.md)
- 📱 [Short Film: 47 Seconds](screenplay/shorts/47-seconds/script.md)
- 🎮 [Interactive CYOA](interactive/cyoa/master-branching.md)
- 🎨 [Storyboard Prompts](visual/storyboards/)

## Project Status

| Component | Status | Version |
|-----------|--------|---------|
| Novella (4-voice) | ✅ Complete | v1 |
| Novella (Diary) | ✅ Complete | v1 |
| Feature Screenplay | ✅ Complete | v1 |
| Short Film Script | ✅ Complete | v1 |
| CYOA Interactive | ✅ Complete | v1 |
| Storyboards | ✅ Complete | v1 |

## Story Summary

[Brief 2-3 paragraph summary]

## How to Navigate

[Instructions for new readers/collaborators]
```

### Directory README Template
```markdown
# [Directory Name]

Brief description of what's in this directory.

## Contents

| File | Description | Status |
|------|-------------|--------|
| file1.md | What it is | ✅ Complete |
| file2.md | What it is | 🚧 Draft |

## Notes

Any special instructions or context.
```

---

## .gitignore SUGGESTIONS

```gitignore
# Generated images (large files)
visual/generated/*.png
visual/generated/*.jpg
*.psd
*.ai

# Word/PDF exports (generate from markdown)
*.docx
*.pdf

# OS files
.DS_Store
Thumbs.db

# Editor files
*.swp
*~
.vscode/
.idea/

# Temporary/working files
*.tmp
*-TEMP.md
scratch/

# Large media files (use Git LFS or external storage)
*.mp4
*.mov
*.wav
*.mp3
```

---

## WORKFLOW RECOMMENDATIONS

### Adding New Content
1. Create feature branch: `git checkout -b feature/new-short-film`
2. Add files in appropriate directory
3. Update relevant README.md files
4. Commit with clear message: `[ADD] Short film 02: The Boyfriend`
5. Push and create PR (if collaborating) or merge to develop

### Making Revisions
1. Create branch: `git checkout -b fix/timeline-consistency`
2. Make changes
3. Update CHANGELOG.md
4. Commit: `[FIX] Correct Alex/Kira meeting date`
5. Merge to develop, then main when stable

### Preparing for Submission
1. Create release branch: `git checkout -b release/new-yorker`
2. Final polish, export to required format
3. Tag: `git tag new-yorker-submitted-2024-01`
4. Archive submission version
5. Merge back to main

---

## MIGRATION PLAN

### Step 1: Initialize Repository Structure
```bash
mkdir -p the-drugfluencer/{docs,characters,world/locations,world/technology}
mkdir -p the-drugfluencer/narrative/{plot-architecture,novellas/v1-four-voices,novellas/v2-the-diary,short-stories}
mkdir -p the-drugfluencer/screenplay/{feature,shorts/47-seconds,series-bible}
mkdir -p the-drugfluencer/interactive/{cyoa,endings,game-design}
mkdir -p the-drugfluencer/visual/{storyboards/prompts-by-scene,mood-boards,generated,style-guides}
mkdir -p the-drugfluencer/audio
mkdir -p the-drugfluencer/production/{budget-estimates,casting-notes,location-scouting}
mkdir -p the-drugfluencer/marketing/{synopsis,pitch-deck,social-strategy}
mkdir -p the-drugfluencer/archive/deprecated
```

### Step 2: Move Existing Files
```bash
# Novella
mv THE_DRUGFLUENCER_Novella.docx narrative/novellas/v1-four-voices/
mv THE_DIARY_New_Yorker_Full_Length.md narrative/novellas/v2-the-diary/the-diary-full.md

# Screenplay
mv THE_DRUGFLUENCER_Screenplay.docx screenplay/feature/
mv THE_DRUGFLUENCER_Short_Film_47_Seconds.md screenplay/shorts/47-seconds/script.md

# Interactive
mv THE_DRUGFLUENCER_Choose_Your_Own_Adventure.md interactive/cyoa/master-branching.md

# Visual
mv THE_DRUGFLUENCER_Storyboard_Prompts_Nihonga.md visual/storyboards/prompts-nihonga.md
mv THE_DRUGFLUENCER_Storyboard_Prompts_Cinematic.md visual/storyboards/prompts-cinematic.md

# Plot
mv THE_DRUGFLUENCER_Plot_Map.md narrative/plot-architecture/master-plot-map.md
```

### Step 3: Create Core Documentation
- Write PROJECT_BIBLE.md (master reference)
- Write TIMELINE.md (chronological events)
- Create character files from existing material
- Add README.md files to each directory

### Step 4: Initial Commit
```bash
git add .
git commit -m "[META] Initial repository structure with all existing materials"
git tag v0.1.0
```

---

## COLLABORATION NOTES

If working with others:

### Protected Branches
- `main` — Requires PR review
- `develop` — Direct push OK for small changes

### Code Owners (CODEOWNERS file)
```
# Default owner
* @your-username

# Specific areas
/narrative/ @writer-collaborator
/visual/ @artist-collaborator
/production/ @producer-collaborator
```

### PR Template
```markdown
## What Changed
Brief description

## Type
- [ ] New content
- [ ] Revision
- [ ] Fix
- [ ] Structure/organization

## Checklist
- [ ] README updated if needed
- [ ] Cross-references checked
- [ ] No broken links
- [ ] CHANGELOG updated (if significant)
```

---

*End of Repository Structure Plan*
