# Sinar Profile README — Maintenance Guide

This directory (`profile/`) contains the Sinar GitHub org profile visible at
`github.com/Sinar`. The content is split into three files for layered
readability.

---

## File structure

```
profile/
├── README.md        # Domain-based project grouping (interest-first)
├── ECOSYSTEMS.md    # Comprehensive Go + Python tech catalog
└── PLONE.md         # Per-site Plone package tree view
```

---

## Architecture

### README.md — Domain view (interest-first)

Beginners pick a topic, not a tech stack. Each section groups repos by
domain, tagged with difficulty and language badges.

**Sections in order:**

| # | Section | Difficulty | Type |
|---|---------|------------|------|
| 1 | Content & Open Data | 🟢 | Non-technical |
| 2 | Open Government | 🟡 | Mixed (Go + Python) |
| 3 | Fellowship Projects | 🟡 | Mixed |
| 4 | Internet Censorship | 🟡 | Mixed |
| 5 | Freedom of Information | 🟡 | Plone |
| 6 | Procurement & Transparency | 🔴 | Plone |
| 7 | Data Analysis & Tools | 🟡 | Mixed |
| 8 | Civic Tech Tools | 🟡 | mySociety forks |

### ECOSYSTEMS.md — Tech catalog (stack-first)

For contributors who already know their language/framework.

| Section | Scope | Count |
|---------|-------|-------|
| Go Ecosystem | All public non-archived Go repos | 6 |
| Python — Plone CMS | Websites, content types, themes, infra | ~36 |
| Python — Django Apps | Django-based web apps | 4 |
| Python — Other Tools | Scripts, scrapers, utilities | ~6 |
| Archive Appendix | Notable archived repos with successor links | ~15 |

### PLONE.md — Per-site Plone trees

Each website's buildout dependencies as a navigable tree with links.

---

## Rules

### Inclusion

- **Only public, non-archived repos** in active listings
- **Private repos** must never appear (e.g., `knowledgemgmt`)
- **Archived repos** go in the Archive Appendix in ECOSYSTEMS.md only
- **Overlap is allowed** — same repo can appear in multiple sections
  (helps beginners discover repos from different angles)

### Exclusions

- `foe-km`, `foecluster.km` — excluded by maintainer request
- Any repo with no push in 5+ years unless it's still relevant
- DevOps/internal repos (e.g., `devops`, `devops-etckeeper`)

---

## Badge conventions

| Badge | Meaning | When to use |
|-------|---------|-------------|
| `[Go]` | Go language | Repo primary language is Go |
| `[Python]` | Python | Repo primary language is Python |
| `[Django]` | Django framework | Repo imports Django (check setup.py/cfg) |
| ⭐ | Actively maintained | Push within last 12 months |
| ⚠️ | Stale | No push in 2+ years but still non-archived |

Difficulty badges appear only in README.md section headers:

| Badge | Meaning |
|-------|---------|
| 🟢 | Beginner-friendly, no code needed |
| 🟡 | Some programming experience |
| 🔴 | Domain expertise (e.g., Plone) |

---

## Data sources (how to verify)

### Language tags (`[Go]` `[Python]` `[Django]`)

```bash
gh repo list Sinar --limit 200 --json name,primaryLanguage,isArchived
```

For Django detection, search for Django patterns in source:

```bash
gh search code "manage.py" --repo Sinar/<repo>
# or check setup.py for "Django" in install_requires
```

### Activity (⭐ / ⚠️)

```bash
gh repo list Sinar --limit 200 --json name,updatedAt,isArchived
```

Compare `updatedAt` against current date. ⭐ = within 1 year.

### Plone buildout dependencies (for PLONE.md)

Read each site's buildout.cfg from GitHub:

```bash
gh api repos/Sinar/<site>/contents/buildout.cfg --jq '.content' | base64 -d
```

Look for `[sources]` (all available packages) and the `[instance]` eggs
list (packages actually enabled).

Known sites with buildout configs:

| Site | Custom package | Buildout URL |
|------|----------------|--------------|
| sinarproject.org | sinarproject.customizations | `.../sinarproject.org/contents/buildout.cfg` |
| imap | imap.customizations | `.../imap/contents/buildout.cfg` |
| enabling-tech | et.customizations | `.../enabling-tech/contents/buildout.cfg` |
| tumpangtanya | tumpangtanya.inforequest | `.../tumpangtanya/contents/buildout.cfg` |
| politikus | politikus.theme | `.../politikus/contents/buildout.cfg` |
| sinar.govdocs | sinar.govdocs | `.../sinar.govdocs/contents/base.cfg` |

### Archive status

```bash
gh repo list Sinar --limit 200 --json name,isArchived
```

Repos with `isArchived: true` must not appear in active listings.

---

## Git discipline

- **Do not commit or push** unless explicitly requested by the maintainer
- Stage only intended files; review `git status` and `git diff` before any commit

## Update workflow

1. **Add a new repo** — decide which domain section(s) it fits, add entry
   with appropriate badges. If it's Go or Python, add to the corresponding
   ECOSYSTEMS.md sub-section too.
2. **Archive a repo** — remove from all active listings, add to the
   Archive Appendix in ECOSYSTEMS.md with the successor link.
3. **Update Plone dependencies** — re-read buildout.cfg for the affected
   site and update the tree view in PLONE.md.
4. **Staleness check** — run quarterly against `gh repo list` to update
   ⭐ and ⚠️ markers.

---

## Cross-file linking

ALWAYS end ECOSYSTEMS.md and PLONE.md with a back-link to README.md:

```markdown
[← Back to README](./README.md)
```
