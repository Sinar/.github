# Plone CMS Ecosystem — Website Package Breakdown

Each Sinar Plone website has a buildout that declares its dependencies. Below is the per-site tree view of which packages are used where.

---

## Legend

| Marker | Meaning |
|--------|---------|
| ⭐ | Actively maintained (push within 1 year) |
| ⚠️ | Plone 5.2 — migration to Plone 6 needed |

---

## Site overview

| # | Site | Plone | Status |
|---|------|-------|--------|
| 1 | [sinarproject.org](#1-sinarprojectorg--sinarprojectcustomizations-) | 6.0 | ⭐ |
| 2 | [imap](#2-imap--imapcustomizations) | 6.0 | |
| 3 | [enabling-tech](#3-enabling-tech--etcustomizations-) | 6.0 | ⭐ |
| 4 | [tumpangtanya](#4-tumpangtanya--tumpangtanyainforequest) | 6.0 | |
| 5 | [politikus](#5-politikus--politikustheme) | 6.0 | |
| 6 | [sinar.govdocs](#6-sinargovdocs--sinargovdocs) | 5.2 | ⚠️ |

---

## 1. sinarproject.org — `sinarproject.customizations` ⭐

Main Sinar Project website. Targets Plone 6.0.

- [sinarproject.org](https://github.com/Sinar/sinarproject.org)
  - **Content Types**
    - [sinar.activity](https://github.com/Sinar/sinar.activity) ⭐
    - [sinar.article](https://github.com/Sinar/sinar.article) ⭐
    - [sinar.indicators](https://github.com/Sinar/sinar.indicators) ⭐
    - [sinar.opportunities](https://github.com/Sinar/sinar.opportunities) ⭐
    - [sinar.organization](https://github.com/Sinar/sinar.organization) ⭐
    - [sinar.project](https://github.com/Sinar/sinar.project) ⭐
    - [sinar.resource](https://github.com/Sinar/sinar.resource) ⭐
  - **Behaviors**
    - [sinar.miscbehavior](https://github.com/Sinar/sinar.miscbehavior) ⭐
  - **Theme**
    - [sinarproject.customizations](https://github.com/Sinar/sinarproject.customizations) ⭐
  - **Vocabularies**
    - [collective.vocabularies.iso](https://github.com/Sinar/collective.vocabularies.iso) ⭐

## 2. imap — `imap.customizations`

Internet censorship monitoring website. Targets Plone 6.0.

- [imap](https://github.com/Sinar/imap)
  - **Content Types**
    - [sinar.activity](https://github.com/Sinar/sinar.activity) ⭐
    - [sinar.advisory](https://github.com/Sinar/sinar.advisory)
    - [sinar.article](https://github.com/Sinar/sinar.article) ⭐
    - [sinar.indicators](https://github.com/Sinar/sinar.indicators) ⭐
    - [sinar.organization](https://github.com/Sinar/sinar.organization) ⭐
    - [sinar.project](https://github.com/Sinar/sinar.project) ⭐
    - [sinar.resource](https://github.com/Sinar/sinar.resource) ⭐
  - **Behaviors**
    - [sinar.miscbehavior](https://github.com/Sinar/sinar.miscbehavior) ⭐
  - **Theme**
    - [imap.customizations](https://github.com/Sinar/imap.customizations)
  - **Vocabularies**
    - [collective.vocabularies.iso](https://github.com/Sinar/collective.vocabularies.iso) ⭐

## 3. enabling-tech — `et.customizations` ⭐

Enabling Tech website. Targets Plone 6.0.

- [enabling-tech](https://github.com/Sinar/enabling-tech)
  - **Content Types**
    - [sinar.activity](https://github.com/Sinar/sinar.activity) ⭐
    - [sinar.article](https://github.com/Sinar/sinar.article) ⭐
    - [sinar.coalition](https://github.com/Sinar/sinar.coalition) ⭐
    - [sinar.indicators](https://github.com/Sinar/sinar.indicators) ⭐
    - [sinar.opportunities](https://github.com/Sinar/sinar.opportunities) ⭐
    - [sinar.organization](https://github.com/Sinar/sinar.organization) ⭐
    - [sinar.project](https://github.com/Sinar/sinar.project) ⭐
    - [sinar.resource](https://github.com/Sinar/sinar.resource) ⭐
  - **Behaviors**
    - [sinar.miscbehavior](https://github.com/Sinar/sinar.miscbehavior) ⭐
  - **Theme**
    - [et.customizations](https://github.com/Sinar/et.customizations) ⭐
  - **Vocabularies**
    - [collective.vocabularies.iso](https://github.com/Sinar/collective.vocabularies.iso) ⭐

## 4. tumpangtanya — `tumpangtanya.inforequest`

FOI request platform. Targets Plone 6.0.

- [tumpangtanya](https://github.com/Sinar/tumpangtanya)
  - **Content Types**
    - [sinar.activity](https://github.com/Sinar/sinar.activity) ⭐
    - [sinar.advisory](https://github.com/Sinar/sinar.advisory)
    - [sinar.organization](https://github.com/Sinar/sinar.organization) ⭐
    - [sinar.project](https://github.com/Sinar/sinar.project) ⭐
    - [sinar.resource](https://github.com/Sinar/sinar.resource) ⭐
    - [tumpangtanya.inforequest](https://github.com/Sinar/tumpangtanya.inforequest)
  - **Behaviors**
    - [sinar.miscbehavior](https://github.com/Sinar/sinar.miscbehavior) ⭐

## 5. politikus — `politikus.theme`

Procurement & political elite research platform. Targets Plone 6.0.

- [politikus](https://github.com/Sinar/politikus)
  - **Content Types**
    - [politikus.contenttypes](https://github.com/Sinar/politikus.contenttypes) ⭐
    - [politikus.extractives](https://github.com/Sinar/politikus.extractives) ⭐
    - [politikus.bods](https://github.com/Sinar/politikus.bods)
    - [politikus.naturalresource](https://github.com/Sinar/politikus.naturalresource)
    - [ocds.contenttypes](https://github.com/Sinar/ocds.contenttypes) ⭐
    - [popolo.contenttypes](https://github.com/Sinar/popolo.contenttypes) ⭐
  - **Theme**
    - [politikus.theme](https://github.com/Sinar/politikus.theme)
  - **Vocabularies**
    - [collective.vocabularies.iso](https://github.com/Sinar/collective.vocabularies.iso) ⭐

## 6. sinar.govdocs — `sinar.govdocs`

Government documents archive. Targets Plone 5.2 ⚠️ — migration to Plone 6 needed.

- [sinar.govdocs](https://github.com/Sinar/sinar.govdocs) ⚠️ Plone 5.2 — upgrade pending

---

## Shared packages across all sites

These are available in `sinarngo.buildout` and used by multiple sites:

| Package | Used by |
|---------|---------|
| `sinarngo` ⭐ | All sites (parent package) |
| `collective.vocabularies.iso` ⭐ | sinarproject.org, imap, enabling-tech, politikus |
| `sinar.miscbehavior` ⭐ | All sites except politikus |

---

[← Back to README](./README.md) · [← ECOSYSTEMS.md](./ECOSYSTEMS.md)
