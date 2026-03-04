# SEO Machine — Hero Network Setup

This is the Hero Network instance of SEO Machine. All context files have been customized for Hero Network.

## Status

**Context Files**: ✅ Complete
**Competitors Config**: ✅ Complete
**Writing Examples**: ✅ Draft (no published blog content yet — update as articles publish)
**Internal Links Map**: ⚠️ Partial — no blog content yet; product/pricing URLs need confirmation
**Data Integrations**: ❌ Not configured (GA4, Search Console, DataForSEO)
**WordPress Integration**: ❌ Not configured (no blog CMS yet)

---

## Quick Start — First Blog Posts

Since we're starting from zero, here's the recommended first content order:

### Priority 1: Foundation Pieces (establish topical authority)
1. `/research video marketing for small business` → `/write video marketing for small business`
2. `/research how to create consistent video content` → `/write how to create consistent video content`
3. `/research linkedin video strategy` → `/write linkedin video strategy for business owners`

### Priority 2: High-Intent Commercial
4. `/research outsource video editing` → `/write should you outsource video editing`
5. `/research done for you video content` → `/write done for you video content vs diy`

### Priority 3: Differentiation Content
6. `/research authentic video content` → `/write why authentic video outperforms polished production`
7. `/research video production without crew` → `/write how to create professional video without a production crew`

---

## Context Files Overview

| File | Status | Notes |
|------|--------|-------|
| `brand-voice.md` | ✅ Complete | Based on Matt's LinkedIn voice profile |
| `features.md` | ✅ Complete | All product features and benefits |
| `target-keywords.md` | ✅ Complete | 6 keyword clusters, BOFU keywords, gaps |
| `competitor-analysis.md` | ✅ Complete | Descript, Opus, Vidyard, agencies |
| `internal-links-map.md` | ⚠️ Partial | No blog content yet; update as articles publish |
| `style-guide.md` | ✅ Complete | Grammar, formatting, terminology |
| `seo-guidelines.md` | ✅ Complete | Keyword rules, meta standards, structure |
| `writing-examples.md` | ⚠️ Draft | Using LinkedIn posts; add blog examples when available |

---

## GitHub

**Source**: https://github.com/TheCraigHewitt/seomachine  
**Hero Network fork**: TODO — re-authenticate `gh` CLI then run: `gh repo fork TheCraigHewitt/seomachine --fork-name hero-seomachine`

**Note**: GitHub token expired (March 2026). Re-auth with `gh auth login` before forking.

---

## Integrations Setup (When Ready)

### Google Search Console
- Follow `data_sources/README.md`
- Will unlock `/research-performance` and real ranking data

### GA4
- Follow `data_sources/README.md`
- Will unlock traffic and conversion data for content decisions

### DataForSEO
- Optional but powerful for SERP analysis
- API key needed — see `data_sources/README.md`

### WordPress
- Only needed if heronetwork.io runs WordPress
- If on another CMS, use `/publish-draft` output and publish manually

---

## Workflow Reminder

```
/research [topic]          ← Always start here
/write [topic]             ← Generates + auto-triggers 4 agents
/optimize [draft file]     ← Final SEO polish
Review + publish manually  ← Until WordPress integration is live
```

---

*Created: March 2026 by Jarvis*
