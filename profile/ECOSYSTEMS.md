# Go & Python Ecosystems

Comprehensive catalog of all public, non-archived Go and Python repositories in the Sinar Project.

---

## Legend

| Badge | Meaning |
|-------|---------|
| ⭐ | Actively maintained (push within 1 year) |
| ⚠️ | Stale — no updates in 2+ years |

---

## Go Ecosystem

6 public repos. All Go-based CLI tools for document processing and data extraction.

| Repo | Description | Last push | Also in |
|------|-------------|-----------|---------|
| [go-electdocs](https://github.com/Sinar/go-electdocs) ⭐ | Election data extraction tools for EC | Apr 2026 | Open Gov |
| [go-pardocs](https://github.com/Sinar/go-pardocs) ⭐ | Parliament PDF → accessible format | Dec 2025 | Open Gov |
| [go-camelot](https://github.com/Sinar/go-camelot) | PDF table detection (clean-room implementation) | Jun 2023 | |
| [go-akomantoso](https://github.com/Sinar/go-akomantoso) | AkomaNtoso XML libraries for par/docs | Oct 2023 | |
| [go-dundocs](https://github.com/Sinar/go-dundocs) | State Assembly debates & questions processing | Oct 2020 | Open Gov |
| [go-oscv3](https://github.com/Sinar/go-oscv3) ⚠️ | Standalone tool for OSCv3 data lifecycle | Jun 2019 | |

---

## Python Ecosystem

47 public, non-archived Python repos. Split into three sub-ecosystems: Plone CMS, Django Apps, and Other Tools. New to Python contributing? Check out [From Web to Data — A contributor's guide to open source Python](https://docs.google.com/presentation/d/1opU1dT9zAy8j6xQ5mt7LGdH72tkUcmbbD1vlViE2IpA/edit?slide=id.g89d9d5ffe4_0_77#slide=id.g89d9d5ffe4_0_77).

### Plone CMS

Sinar runs several websites on [Plone](https://plone.org/) 6. The shared buildout (`sinarngo.buildout`) declares dependencies; each site enables a subset of packages.

#### Websites

| Site | Custom package | Description |
|------|----------------|-------------|
| [sinarproject.org](https://github.com/Sinar/sinarproject.org) | [sinarproject.customizations](https://github.com/Sinar/sinarproject.customizations) | Main Sinar Project website |
| [imap](https://github.com/Sinar/imap) | [imap.customizations](https://github.com/Sinar/imap.customizations) | iMAP internet censorship monitoring |
| [enabling-tech](https://github.com/Sinar/enabling-tech) | [et.customizations](https://github.com/Sinar/et.customizations) | Enabling Tech |
| [tumpangtanya](https://github.com/Sinar/tumpangtanya) | [tumpangtanya.inforequest](https://github.com/Sinar/tumpangtanya.inforequest) | FOI request platform |
| [politikus](https://github.com/Sinar/politikus) | [politikus.theme](https://github.com/Sinar/politikus.theme) | Procurement & political elite research |
| [sinar.govdocs](https://github.com/Sinar/sinar.govdocs) | [sinar.govdocs](https://github.com/Sinar/sinar.govdocs) | Government documents archive (Plone 5.2) |

#### Reusable Content Types

| Package | Description | Last push |
|---------|-------------|-----------|
| [sinar.organization](https://github.com/Sinar/sinar.organization) | Organization content type | Apr 2026 |
| [sinar.project](https://github.com/Sinar/sinar.project) ⭐ | Project folderish content type | Apr 2026 |
| [sinar.activity](https://github.com/Sinar/sinar.activity) ⭐ | Activity content type for civil society | Apr 2026 |
| [sinar.article](https://github.com/Sinar/sinar.article) ⭐ | Folderish page for short updates/blogs | Apr 2026 |
| [sinar.resource](https://github.com/Sinar/sinar.resource) ⭐ | Generic Resource content type | Apr 2026 |
| [sinar.opportunities](https://github.com/Sinar/sinar.opportunities) ⭐ | Opportunities content add-on | Apr 2026 |
| [sinar.coalition](https://github.com/Sinar/sinar.coalition) ⭐ | Coalitions & networks of organizations | May 2025 |
| [sinar.corruptiontracker](https://github.com/Sinar/sinar.corruptiontracker) ⭐ | Corruption issue tracking | May 2026 |
| [sinar.indicators](https://github.com/Sinar/sinar.indicators) ⭐ | M&E indicators add-on | Apr 2026 |
| [sinar.advisory](https://github.com/Sinar/sinar.advisory) | Input/feedback/recommendations content type | Jan 2023 |
| [sinar.digimon](https://github.com/Sinar/sinar.digimon) | Digital Rights Incident Reporting | Jul 2022 |
| [sinar.pardocs](https://github.com/Sinar/sinar.pardocs) | Plone extensions for Parliamentary Documents | Sep 2023 |
| [sinar.miscbehavior](https://github.com/Sinar/sinar.miscbehavior) ⭐ | Miscellaneous behaviors for content types | Apr 2026 |
| [sinar.popit](https://github.com/Sinar/sinar.popit) ⚠️ | Plone portlets/behaviors for popit databases | Apr 2018 |
| [popolo.contenttypes](https://github.com/Sinar/popolo.contenttypes) ⭐ | Popolo standard content types | Mar 2026 |
| [ocds.contenttypes](https://github.com/Sinar/ocds.contenttypes) ⭐ | OCDS-compliant contract transparency types | Mar 2026 |
| [politikus.contenttypes](https://github.com/Sinar/politikus.contenttypes) ⭐ | Core content types for Politikus platform | Mar 2026 |
| [politikus.extractives](https://github.com/Sinar/politikus.extractives) ⭐ | Extractive industry concessions tracking | Mar 2026 |
| [politikus.bods](https://github.com/Sinar/politikus.bods) | Beneficial Ownership Data Standards | May 2024 |
| [politikus.naturalresource](https://github.com/Sinar/politikus.naturalresource) | Natural resource information tracking | Jun 2021 |

#### Vocabularies

| Package | Description | Last push |
|---------|-------------|-----------|
| [collective.vocabularies.iso](https://github.com/Sinar/collective.vocabularies.iso) ⭐ | ISO code vocabularies for Plone | Apr 2026 |

#### Themes & Customizations

| Package | For site | Last push |
|---------|----------|-----------|
| [sinarproject.customizations](https://github.com/Sinar/sinarproject.customizations) ⭐ | sinarproject.org | Apr 2026 |
| [imap.customizations](https://github.com/Sinar/imap.customizations) | imap | Sep 2024 |
| [et.customizations](https://github.com/Sinar/et.customizations) ⭐ | enabling-tech | Jan 2026 |
| [nmg.unmasked.views](https://github.com/Sinar/nmg.unmasked.views) ⚠️ | NMG Unmasked portal | Oct 2020 |
| [sinarngo](https://github.com/Sinar/sinarngo) ⭐ | Parent package (shared utilities) | Feb 2026 |

#### Infrastructure

| Package | Description | Last push |
|---------|-------------|-----------|
| [sinarngo.buildout](https://github.com/Sinar/sinarngo.buildout) | Shared Plone buildout | Oct 2022 |
| [documents.buildout](https://github.com/Sinar/documents.buildout) | Plone buildout for document sites | Jun 2023 |
| [sinarplone-docker](https://github.com/Sinar/sinarplone-docker) ⭐ | Docker environment for Plone 5 | Apr 2026 |

---

### Django Apps

| Repo | Description | Framework | Last push | Status |
|------|-------------|-----------|-----------|--------|
| [popit_ng](https://github.com/Sinar/popit_ng) ⭐ | Popolo reps database + REST API | Django 1.11 + DRF | May 2026 | Active |
| [blockedornot](https://github.com/Sinar/blockedornot) ⭐ | Internet censorship checker | Django | Jul 2025 | Active |
| [legisdata](https://github.com/Sinar/legisdata) | Parliamentary data + SayIt frontend | Django | Jul 2024 | Active |
| [contractit](https://github.com/Sinar/contractit) ⚠️ | Contract storage backend with API | Django | May 2018 | Stale |

---

### Other Python Tools

| Repo | Description | Last push | Status |
|------|-------------|-----------|--------|
| [mapit](https://github.com/Sinar/mapit) ⭐ | Postcode-to-boundary API (mySociety fork) | Jun 2025 | Active |
| [popit_relationship](https://github.com/Sinar/popit_relationship) ⭐ | Graph-based rep relationship analysis | Mar 2026 | Active |
| [camelot](https://github.com/Sinar/camelot) ⚠️ | PDF table extraction library | Dec 2021 | Stale |
| [myprocurement-scrapers](https://github.com/Sinar/myprocurement-scrapers) ⚠️ | MyProcurement data scrapers | Feb 2021 | Stale |
| [openownership-scripts](https://github.com/Sinar/openownership-scripts) ⚠️ | Open Ownership data scripts | Feb 2022 | Stale |
| [BillWatcher-2.0](https://github.com/Sinar/BillWatcher-2.0) ⚠️ | Parliament bill tracker | Sep 2020 | Stale |
| [sinarproject.customizations](https://github.com/Sinar/sinarproject.customizations) ⭐ | (listed under Plone above) | Apr 2026 | Active |

---

## Archive Appendix

Notable archived repos that provide reference or migration context for active projects.

| Archived repo | Relates to | Why it matters |
|---------------|------------|----------------|
| [popit_ng-docker](https://github.com/Sinar/popit_ng-docker) | popit_ng | Docker deployment reference |
| [popit-scripts](https://github.com/Sinar/popit-scripts) | popit_ng | Data import/sync patterns |
| [popit.dicapati](https://github.com/Sinar/popit.dicapati) | popit_ng | Business rules & data integrity |
| [popit_Gsheet_sync](https://github.com/Sinar/popit_Gsheet_sync) | popit_ng | Google Sheets sync approach |
| [wakilrakyat.buildout](https://github.com/Sinar/wakilrakyat.buildout) | popolo / popit_ng | Legacy representatives site buildout |
| [sinarngo.organization](https://github.com/Sinar/sinarngo.organization) ⚡ | sinar.organization | Predecessor content type |
| [sinarngo.project](https://github.com/Sinar/sinarngo.project) ⚡ | sinar.project | Predecessor content type |
| [sinarngo.activity](https://github.com/Sinar/sinarngo.activity) ⚡ | sinar.activity | Predecessor content type |
| [sinarngo.resource](https://github.com/Sinar/sinarngo.resource) ⚡ | sinar.resource | Predecessor content type |
| [sinar.citation](https://github.com/Sinar/sinar.citation) | sinar.content types | Reference for citation content type pattern |
| [sinar.foi](https://github.com/Sinar/sinar.foi) | tumpangtanya | Legacy FOI approach |
| [ocds-scripts](https://github.com/Sinar/ocds-scripts) | ocds.contenttypes | Legacy OCDS data conversion |
| [malaysian-elections](https://github.com/Sinar/malaysian-elections) | go-electdocs | Historical election data |
| [sinar.myreps](https://github.com/Sinar/sinar.myreps) | popit_ng | Legacy representative lookup |
| [sinar.electorallookup](https://github.com/Sinar/sinar.electorallookup) | popit_ng | Legacy electoral boundary lookup |

> ⚡ denotes repos with recent activity (2024-12) that were archived in the bulk archiving pass — the code may still have useful patterns.

---

[← Back to README](./README.md)
