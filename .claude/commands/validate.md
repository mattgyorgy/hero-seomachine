# Validate Command

Use this command to audit any article against the 7 Issues framework and hard requirements from @context/rules.md.

## Usage
`/validate [file-path]`

## What This Command Does
1. Loads the article and extracts frontmatter (meta title, description, keywords)
2. Checks the article against all 7 Issues from @context/rules.md
3. Scores each issue (PASS, WARNING, FAIL)
4. Provides specific fix recommendations for any failures
5. Outputs a validation report with action items

## Process

### Step 1: Load and Parse Article
- Read the markdown file from `drafts/`, `published/`, or specified path
- Extract frontmatter: Meta Title, Meta Description, Primary Keyword, Secondary Keywords, Word Count
- Parse content structure: H1, H2s, H3s, paragraphs, lists, bold text, links

### Step 2: Issue #1 — Generic Introductions Audit

**Check for forbidden openers:**
- [ ] "In today's digital landscape..."
- [ ] "[Topic] has become increasingly important..."
- [ ] "Many businesses struggle with..."
- [ ] "This comprehensive guide will explore..."
- [ ] "As we all know..."
- [ ] "When it comes to..."

**Check for required elements in first paragraph:**
- [ ] Specific data point, OR
- [ ] Contrarian statement, OR
- [ ] Case study opener with name and scenario

**Scoring:**
- **PASS**: No forbidden patterns + has specific hook
- **WARNING**: 1 forbidden pattern OR weak hook
- **FAIL**: 2+ forbidden patterns OR generic definition opening

**Fix recommendation if FAILED:**
```
Issue #1 FAILED — Generic Introduction Detected

Problem: Article opens with [forbidden pattern found]

Fix: Rewrite first paragraph to start with ONE of:
- Specific data point ("We spent $X before realizing...")
- Contrarian statement ("The bottleneck isn't X, it's Y...")
- Case study opener ("[Name]'s agency had [specific scenario]...")

Example rewrite:
[Show before → after example]
```

### Step 3: Issue #2 — Wikipedia-Style Structure Audit

**Check H2 structure for generic patterns:**
- [ ] NO "What is [Topic]?"
- [ ] NO "Why [Topic] Matters"
- [ ] NO "Benefits of [Topic]"
- [ ] NO "How to [Topic]" (unless it's a pure how-to query)
- [ ] NO "Best Practices"

**Check section depth:**
- [ ] Each H2 has 300+ words
- [ ] No H2 with <200 words (too shallow)
- [ ] Structure matches user journey

**Scoring:**
- **PASS**: No generic H2s + all sections 300+ words
- **WARNING**: 1 generic H2 OR 1 section <300 words
- **FAIL**: 2+ generic H2s OR multiple shallow sections

**Fix recommendation if FAILED:**
```
Issue #2 FAILED — Wikipedia-Style Structure

Problem: Found generic H2s: [list]

Fix: Restructure based on user journey:
- How-to queries → Start with process steps
- Problem-solving → Symptoms → Diagnosis → Solution
- Comparison → Criteria → Side-by-side → Recommendation

Example rewrite:
[Show current H2s → recommended H2s]
```

### Step 4: Issue #3 — E-E-A-T Signals Audit

**Check for experience markers (every 500 words):**
- [ ] "In our analysis of X..." or first-hand experience
- [ ] Specific customer scenario with name (Marcus Chen, Sarah Mercer)
- [ ] Industry data with cited source
- [ ] Concrete numbers or timeframes
- [ ] Screenshots or results descriptions

**Count E-E-A-T signals:**
- Word count ÷ 500 = minimum required signals
- Example: 2,500 words = minimum 5 signals

**Scoring:**
- **PASS**: Meets or exceeds signal count requirement
- **WARNING**: 1-2 signals below requirement
- **FAIL**: 3+ signals below requirement OR zero signals

**Fix recommendation if FAILED:**
```
Issue #3 FAILED — Missing E-E-A-T Signals

Required: [X] signals (word count ÷ 500)
Found: [Y] signals

Fix: Add experience markers every 500 words:
- "In our analysis of 200+ agency workflows..."
- "Marcus Chen's content agency had [specific scenario]..."
- "HubSpot's Agency Pricing Report found [data]..."

Missing signal locations:
[Show word count markers where signals should be added]
```

### Step 5: Issue #4 — Statistical Averages Problem Audit

**Check for differentiation elements:**
- [ ] Original methodology or framework mentioned
- [ ] Contrarian take with supporting evidence
- [ ] Proprietary data or specific constraints
- [ ] Takes a position (not just summarizes consensus)

**Scoring:**
- **PASS**: Has 1+ differentiation element
- **WARNING**: Weak differentiation (safe, consensus-driven)
- **FAIL**: Pure summary of common advice with no unique angle

**Fix recommendation if FAILED:**
```
Issue #4 FAILED — Statistical Averages Problem

Problem: Article reads like summary of common advice. No unique perspective.

Fix: Add ONE of:
- Original framework ("3-layer approach to X...")
- Contrarian angle ("Most agencies get X wrong because...")
- Proprietary data ("After processing 1,000 videos, we found...")
- Specific constraints ("This only works if you...")
```

### Step 6: Issue #5 — Keyword Stuffing Patterns Audit

**Count primary keyword usage:**
- [ ] Total uses: [count] (target: 3-5)
- [ ] Placement check:
  - [ ] H1: [present/absent]
  - [ ] First 100 words: [present/absent]
  - [ ] Last paragraph: [present/absent]
  - [ ] H2s: [count of H2s with keyword]

**Check for unnatural density:**
- [ ] No paragraph with keyword used >2 times
- [ ] No sentence reads awkwardly to force keyword

**Scoring:**
- **PASS**: 3-5 uses with natural placement
- **WARNING**: 6-8 uses OR slightly awkward placement
- **FAIL**: 9+ uses OR clearly forced placement

**Fix recommendation if FAILED:**
```
Issue #5 FAILED — Keyword Stuffing Detected

Problem: Primary keyword used [X] times (target: 3-5)
Overused locations: [list specific paragraphs/locations]

Fix: Reduce to 3-5 natural uses. Replace excess with synonyms:
- "remote video production" → "producing video remotely"
- "remote video production" → "remote production workflow"
- "remote video production" → "video production at a distance"

Keep only these placements:
- H1 (1 use)
- First 100 words (1 use)
- Last paragraph (1 use)
- 1-2 H2s (natural fit only)
```

### Step 7: Issue #6 — Internal Linking Strategy Audit

**Count and evaluate internal links:**
- [ ] Total internal links: [count] (target: 3-5)
- [ ] Contextual placement (not just "learn more")
- [ ] Descriptive anchor text
- [ ] Links to relevant pillar content

**Scoring:**
- **PASS**: 3-5 contextual internal links
- **WARNING**: 2 links OR generic anchor text
- **FAIL**: 0-1 links OR all links generic

**Fix recommendation if FAILED:**
```
Issue #6 FAILED — Weak Internal Linking

Problem: Only [X] internal links found / Generic anchor text
Current links: [list with anchor text]

Fix: Add 3-5 contextual links with descriptive anchor:
- Replace "learn more" → "remote video production workflow"
- Replace "click here" → "agency video scaling strategies"
- Link to related articles and product pages naturally
```

### Step 8: Issue #7 — User Engagement Signals Audit ⭐ CRITICAL

**Check paragraph structure:**
- [ ] Max 2-3 sentences per paragraph
- [ ] No walls of text (>4 lines on desktop)

**Count visual breaks (bullets, bold, lists, quotes):**
- Word count ÷ 350 = minimum required visual breaks
- Example: 2,800 words = minimum 8 visual breaks

**Check for specific elements:**
- [ ] Bullet point lists: [count] (minimum 2 sections)
- [ ] Bold key takeaways: [count] (minimum 3-5 per article)
- [ ] Numbered steps: [present/absent]
- [ ] Discussion prompt or question: [present/absent]

**Scoring:**
- **PASS**: All paragraph rules met + visual break quota + elements present
- **WARNING**: 1-2 minor violations (e.g., 1 paragraph with 4 sentences)
- **FAIL**: Multiple violations OR missing key engagement elements

**Fix recommendation if FAILED:**
```
Issue #7 FAILED — Poor User Engagement Signals

Problems found:
- [X] paragraphs exceed 3 sentences
- Only [Y] visual breaks (need [Z])
- Missing: [bullet lists / bold takeaways / discussion prompt]

Fix: Add engagement elements:
1. Break long paragraphs into 2-3 sentence chunks
2. Add visual break every 300-400 words:
   - Bullet list for 3+ related items
   - Bold standalone takeaway line
   - Numbered steps for processes
   - Quote block for key insight
3. Add discussion prompt: "What's your biggest video production bottleneck?"

Target metrics:
- Time-on-page: 3+ minutes
- Bounce rate: <45%
```

### Step 9: Meta Elements Audit

**Check frontmatter completeness:**
- [ ] Meta Title: [X] chars (target: 50-60)
- [ ] Meta Description: [X] chars (target: 150-160)
- [ ] Primary Keyword: [present]
- [ ] Secondary Keywords: [present]
- [ ] URL Slug: [present]
- [ ] Word Count: [matches actual count]

**Scoring:**
- **PASS**: All meta elements present and within limits
- **WARNING**: 1-2 minor issues (e.g., title 65 chars)
- **FAIL**: Missing critical elements OR major limit violations

### Step 10: Generate Validation Report

**Calculate Overall Score:**
```
Issues Passed: [X]/7
Issues Warning: [Y]/7
Issues Failed: [Z]/7

Overall Status: [PASS / NEEDS REVIEW / FAIL]

PASS: 0 failures, ≤2 warnings
NEEDS REVIEW: 1-2 failures, or >2 warnings
FAIL: 3+ failures
```

**Generate Action Items:**
List specific fixes in priority order:
1. Critical (Issue #7 failures — engagement signals)
2. High (Issue #1, #3 failures — intros, E-E-A-T)
3. Medium (Issue #2, #4, #5 — structure, differentiation, keywords)
4. Low (Issue #6 — internal linking, meta tweaks)

## Output

### 1. Validation Report File
Save to: `drafts/validation-report-[article-slug]-[YYYY-MM-DD].md`

Contains:
- Overall score and status
- Detailed audit results for each issue
- Specific fix recommendations with examples
- Priority-ranked action items

### 2. Console Summary
Display:
```
========================================
VALIDATION REPORT: [Article Title]
========================================

Overall: [PASS / NEEDS REVIEW / FAIL]
Score: [X]/7 issues passed

CRITICAL ISSUES (Fix First):
- Issue #7: [status] — [brief description]

HIGH PRIORITY:
- Issue #1: [status]
- Issue #3: [status]

MEDIUM PRIORITY:
- Issue #2: [status]
- Issue #4: [status]
- Issue #5: [status]

LOW PRIORITY:
- Issue #6: [status]

Word Count: [X]
Primary Keyword: [keyword] (used [Y] times)

Next Steps:
[Specific action items]
========================================
```

## Validation Rules Summary

| Issue | Check | Target | Critical? |
|-------|-------|--------|-----------|
| #1 | Forbidden openers | 0 patterns | YES |
| #1 | Specific hook | Present | YES |
| #2 | Generic H2s | 0 generic | NO |
| #2 | Section depth | 300+ words each | NO |
| #3 | E-E-A-T signals | WC÷500 minimum | YES |
| #4 | Differentiation | 1+ element | NO |
| #5 | Keyword count | 3-5 uses | NO |
| #5 | Keyword placement | H1, intro, close | YES |
| #6 | Internal links | 3-5 contextual | NO |
| #7 | Paragraph length | Max 2-3 sentences | YES |
| #7 | Visual breaks | WC÷350 minimum | YES |

## Follow-Up Actions

### If PASS (0 failures, ≤2 warnings)
- Article meets quality standards
- Proceed to optimization agents or publish

### If NEEDS REVIEW (1-2 failures, or >2 warnings)
- Review specific failures
- Apply recommended fixes
- Re-run `/validate` after fixes

### If FAIL (3+ failures)
- Significant revision required
- Consider rewriting sections vs. patching
- Re-run `/validate` after major revisions

## Integration with Write Workflow

The `/validate` command can be used:
1. **After `/write`** — validate before optimization agents
2. **Before publishing** — final quality check
3. **On existing content** — audit published articles for improvement
4. **During debugging** — identify issues in underperforming posts

## Reference Documents

Always consult:
- @context/rules.md — Full 7 Issues framework
- @context/brand-voice.md — Tone and messaging
- @context/customer-proof.md — Case study templates
- @context/platform-workflow.md — Accurate terminology
- @context/pricing-details.md — Pricing accuracy
