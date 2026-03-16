# SEO Machine Content Rules

**Purpose**: Hard requirements every article must meet before publication. These rules prevent the common failures of generic AI content.

**Last Updated**: 2026-03-12  
**Source**: Noel Ceta debugging framework + engagement signal research

---

## The 7 Issues Framework (Audit Checklist)

Every article must pass audit against these 7 failure modes:

### Issue #1: Generic Introductions
**What AI writes**: "In today's digital landscape, [topic] has become increasingly important. Many businesses struggle with [problem]. This comprehensive guide will explore..."

**Why it fails**: Every AI post starts identically. No hook. Signals low-quality content immediately. Readers bounce in 3 seconds.

**The Fix**:
Replace with ONE of:
- Specific data point ("We spent $14k on SEO tools before realizing...")
- Contrarian statement ("Video retainers don't fail because of editing quality...")
- Real case study opener ("Marcus Chen's agency had 4 video clients and one producer. Then he tried to add a fifth...")

**Forbidden openers**:
- "In today's digital landscape..."
- "[Topic] has become increasingly important..."
- "Many businesses struggle with..."
- "This comprehensive guide will explore..."
- "As we all know..."

**First paragraph must include**: concrete number, specific timeframe, or real scenario

**Validation**: Read only the first paragraph. Would a busy agency producer keep reading?

---

### Issue #2: Wikipedia-Style Structure (Surface-Level Coverage)
**What AI creates**: What is [Topic], Why [Topic] Matters, Benefits of [Topic], How to [Topic], Best Practices, Conclusion.

**Why it fails**: Predictable structure signals AI pattern. Doesn't match user intent. Broad overviews that touch 10 topics at 100 words each never satisfy search intent.

**The Fix** — Restructure based on actual user journey:

**How-to queries** → Start with process (jump straight into steps)
**Problem-solving queries** → Start with symptoms → diagnosis → solution
**Comparison queries** → Lead with criteria → side-by-side → recommendation

**Structure Rules**:
- Each H2 must cover ONE specific subtopic with depth (minimum 300 words)
- Prefer 3 deep sections over 6 shallow ones
- Include: how-to steps, specific examples, concrete numbers, or real scenarios
- NO generic H2s like "What is X" or "Why X Matters" unless search intent specifically requires definition

**Example restructuring**:
- Before: "What is Remote Video Production? → Benefits → Best Practices → Conclusion"
- After: "The Site Visit Bottleneck → How Guest Upload Links Work → Scaling Without Adding Producers → Real Agency Economics"

**Validation**: Could a reader implement this section after reading it? If not, it's too shallow.

---

### Issue #3: Missing E-E-A-T Signals
**What AI doesn't include**: Personal experience markers, expertise indicators, original research, author credibility.

**Why it fails**: Google's Experience update prioritizes first-hand knowledge. AI content is theoretical, not experiential.

**The Fix** — Add experience markers every 500 words:

**First-hand experience**:
- "In our analysis of 200+ agency workflows..."
- "When we onboarded our 50th video production client..."
- "After processing 1,000+ remote recordings, we noticed..."

**Specific customer scenarios**:
- "Marcus Chen's content agency had 4 video clients and one producer..."
- "Sarah Mercer's marketing team outside Austin tried client self-recording..."

**Screenshots/results**:
- Include descriptions of actual dashboards, workflows, or results
- Reference specific metrics ("Time-on-page improved from 1:12 to 3:47")

**Author credibility**:
- Include brief author/brand bio establishing expertise
- Cite 1-2 authoritative external sources per article

**Validation**: Could this content have been written by someone with no industry experience? If yes, add more signals.

---

### Issue #4: Statistical Averages Problem
**What AI does**: Aggregates info from training data → produces middle-ground advice. Safe, consensus-driven, generic.

**Why it fails**: No unique perspective. Nothing new to add. Google already has thousands of versions saying the same thing.

**The Fix**:
- Add original methodology ("3-layer framework for client onboarding")
- Use contrarian angles with evidence ("Why most agencies get remote video wrong")
- Include proprietary data and specific constraints
- Take a position. Don't just summarize what everyone else says.

**Example**:
- Before: "Remote video production has many benefits including cost savings and flexibility..."
- After: "Remote video production fails at the capture stage, not the edit. Here's the 4-point client briefing that fixes it..."

**Every article needs ONE of**:
- Original framework/methodology
- Contrarian take backed by data
- Specific process others aren't sharing
- Real numbers from actual work

---

### Issue #5: Keyword Stuffing Patterns
**What AI does**: Overuses target keywords, unnatural placement, obvious optimization patterns. "Content marketing strategy" used 47 times in one post.

**Why it fails**: Google's NLP understands context. Unnatural patterns flag AI content. Reads like spam.

**The Fix**:
- Use target keyword 3-5 times naturally per article
- Use synonyms and related terms (LSI keywords)
- Focus on semantic relevance over exact match

**Keyword Placement Rules**:
- H1: Must include primary keyword (naturally)
- First 100 words: Include primary keyword once
- Last paragraph: Include primary keyword once
- 2-3 H2s: Include primary or secondary keyword
- Total: 3-5 primary keyword uses maximum

**Example improvement**:
- Before: "Content marketing strategy" used 47 times
- After: "Content marketing strategy" used 5 times + related terms like "content planning," "editorial approach," "publishing framework"

---

### Issue #6: Missing Internal Linking Strategy
**What AI does**: No internal links or generic "learn more" links.

**Why it fails**: Google can't understand topic relationships → PageRank not distributed effectively. Missed opportunity to build topical authority.

**The Fix**:
- Use hub-spoke model: pillar content links to subtopics
- Add 3-5 contextual internal links per post (not just "learn more")
- Create interlinked topic clusters
- Link to specific articles, not just homepage

**Internal Link Rules**:
- Minimum 2 internal links per article
- Use descriptive anchor text (not "click here")
- Link to related articles in the same cluster
- Link to product/features where contextually relevant

---

### Issue #7: No User Engagement Signals ⭐ CRITICAL
**What AI creates**: Text-only walls. No interaction elements.

**Why it fails**: High bounce rate → low time-on-page → hurts rankings. Google sees users leaving.

**The Fix**:
- Add images every 300-400 words
- Include bullet points and bold key takeaways
- Paragraphs 2-3 sentences max
- Discussion prompts throughout

**Results from Noel Ceta's fixes**:
- Time-on-page: 1:12 → 3:47
- Bounce rate: 68% → 41%
- Rankings improved within 3 weeks

---

### Issue #7 Extended: Engagement Implementation Requirements

**The Fix** (detailed implementation):

#### Visual Breaks (Every 300-400 words)
- Include at least ONE visual element per 400 words:
  - Bullet point list (not just paragraphs)
  - Bold key takeaways (standalone lines)
  - Numbered steps or checklists
  - Quote block with key insight
  - [Image placeholder: describe what image should show]

#### Paragraph Structure
- **Maximum 2-3 sentences per paragraph**
- No walls of text exceeding 4 lines
- Vary paragraph length: mix short punchy (1 sentence) with medium (2-3 sentences)
- One idea per paragraph

#### Scannable Formatting
- Use **bold** for key terms and takeaways (3-5 per section)
- Use bullet points for lists of 3+ related items
- Use numbered lists for sequential steps
- Use H3 subheads within H2 sections (breaks up long sections)

#### Engagement Elements
- Include ONE discussion prompt or question per article
- Include ONE "Action Step" or "Quick Win" callout box concept
- End sections with a transition or hook to next section

**Target Metrics** (based on Noel Ceta research):
- Time-on-page goal: 3+ minutes
- Bounce rate goal: <45%
- If current metrics are worse, prioritize Issue #7 fixes first

---

## CTA Requirements

**What AI creates**: Generic "Contact us to learn more" or no CTA at all.

**Why it fails**: No conversion path. Wasted traffic.

**The Fix**:
- Every article must have a contextual CTA in the conclusion
- CTA must flow naturally from the content (not tacked on)
- For Hero Network content, CTAs should:
  - Reference the specific problem just solved
  - Mention Founder Pricing ($79/mo) when relevant
  - Link to relevant internal page (not just homepage)
  - Be 1-2 sentences max

**Example**: "Remote video production removes the site visit bottleneck. Hero Network's guest upload links let your clients record from their phones — no accounts, no apps. Founder pricing is $79/mo. [See how it works →]"

---

## Hard Requirements Checklist

Every article MUST meet these before publication:

### Structure
- [ ] 2,000-3,500 words (exception: 1,500+ for highly specific tactical posts)
- [ ] Minimum 4 H2 sections
- [ ] Every H2 has 300+ words
- [ ] Paragraphs max 3 sentences
- [ ] Visual break every 300-400 words (bullets, bold, images, etc.)

### Keywords
- [ ] Primary keyword in H1
- [ ] Primary keyword in first 100 words
- [ ] Primary keyword in at least 2 H2s
- [ ] Primary keyword in last paragraph
- [ ] 3-5 secondary keywords distributed naturally
- [ ] Density check: Primary keyword ≤3%

### Links
- [ ] Minimum 2 internal links (to other articles or product pages)
- [ ] 1-2 external authoritative links (industry reports, recognized sources)
- [ ] All links use descriptive anchor text (not "click here")

### E-E-A-T
- [ ] First-hand experience or specific customer scenario included
- [ ] Data/statistics cited with source
- [ ] Concrete numbers or timeframes mentioned
- [ ] Article couldn't have been written by AI without domain knowledge

### Engagement
- [ ] Bullet points in at least 2 sections
- [ ] Bold key takeaways (3-5 per article)
- [ ] One numbered list or step-by-step process
- [ ] Discussion prompt or question included
- [ ] CTA in conclusion that flows from content

### Meta
- [ ] Meta title: 50-60 characters, includes primary keyword
- [ ] Meta description: 150-160 characters, includes primary keyword + value prop
- [ ] URL slug: lowercase, hyphenated, includes primary keyword
- [ ] Image alt text: Descriptive, includes keyword where natural

---

## Debugging Workflow (For Existing Content)

Apply this to underperforming articles (position 15+ in GSC):

1. **Identify**: Pull articles ranking position 15+ with impressions >100 (high potential, low performance)

2. **Audit**: Score each against the 7 Issues (1-5 scale per issue)

3. **Prioritize**: Fix high-impression, low-position posts first

4. **Fix Order**:
   - Quick wins: Rewrite intros (Issue #1) — fastest impact
   - Structure: Add formatting, break up paragraphs (Issue #7)
   - Depth: Expand shallow sections (Issue #2)
   - E-E-A-T: Add experience signals, citations (Issue #3)

5. **Measure**: Track time-on-page and bounce rate improvements

---

## Brand Voice Rules (Hero Network Specific)

These override generic SEO advice:

### Always
- Write to agency producers as peers (not beginners)
- Lead with operational problems (site visits, scheduling, client management)
- Use specific numbers and economics ($79/mo vs $1,500 retainer)
- Position as tool in stack (like Frame.io, Notion)

### Never
- "Game-changing" or "revolutionary"
- "Delve into" or "landscape"
- Explain what a retainer is or why video matters
- Teacher-to-student tone
- Em dashes (--) unless truly necessary
- More than 2 em dashes per article

---

## Quick Reference: Paragraph Rules

| Element | Rule | Why |
|---------|------|-----|
| Sentences per paragraph | Max 3 | Prevents text walls |
| Lines per paragraph | Max 4 on desktop | Visual breathing room |
| Paragraphs between visuals | Max 3 | Keeps scannable |
| Bold takeaways per section | 1-2 | Highlights key points |
| Bullet lists | Use for 3+ related items | Easier to scan |

---

## Success Metrics

Based on Noel Ceta's debugging framework, target these improvements:

| Metric | Before | After | Timeline |
|--------|--------|-------|----------|
| Time-on-page | 1:12 | 3:00+ | 3-4 weeks |
| Bounce rate | 68% | <45% | 3-4 weeks |
| Avg position | 47 | 18 | 4-6 weeks |
| Top 10 rankings | 0 | 20%+ of content | 6-8 weeks |

---

## Key Takeaway

**AI content isn't the problem. Generic, unoptimized AI content is.**

Stop publishing raw AI output. Start debugging with systematic fixes.

Your AI content doesn't need replacement. It needs debugging.

**Results from systematic debugging** (Noel Ceta, 50 posts):
- Total monthly clicks: 200 → 4,800 (+2,300%)
- Average position: 47 → 18
- Posts ranking top 10: 0 → 23
- Time invested: 60 hours total

---

*These rules are non-negotiable. An article that fails 2+ hard requirements goes back to draft.*
