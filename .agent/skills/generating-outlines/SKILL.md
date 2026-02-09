---
name: generating-outlines
description: >
  Generates a comprehensive Semantic SEO outline, focusing on Entity Coverage, Search Intent, and Topical Authority.
  Triggers: create outline, lap dan y, semantic outline, /generate-outline
---

# Generating Outlines

## Purpose
Generates a deep, entity-rich content outline that builds topical authority by covering related entities and answering user intent comprehensively.

## Process

### Phase 1: Semantic Strategy & Discovery

#### Entry Check
```
IF `search-intent.md` exists:
    → Load Intent Data (Micro-Intent, Format, Motivation).
IF target keyword is provided:
    → Proceed to Strategy Definition.
ELSE:
    → Error: Missing Keyword.
```

#### Strategy Definition
*Before outlining, define:*
*   **Target Keyword**: [Primary Keyword]
*   **User Intents**: [Primary Intent from `search-intent.md` + Clusters from `research.md`]
*   **Content Format**: [Recommended Format from `search-intent.md`]
*   **Target Audience**: [Beginner vs Expert]
*   **Primary Entity**: [Main Subject]
*   **Related Entities**: [5-10 key entities to mention]

### Phase 2: Content Structure Generation

#### Structure Template
**I. Header & Meta**
*   **Title**: Keyword + Power Word + Current Year (2026).
*   **Meta Description**: Problem + Solution + Keyword.

**II. Introduction (The Hook)**
*   **H1**: Main Heading.
*   **Hook**: Immediate pain point or curiosity.
*   **Entity Definition**: Quick definition for Google Bot context.
*   **The "Why"**: Benefit to reader.

**III. Main Body (Topical Depth)**
*Constraint*: Create an H2 for *every* distinct intent or query cluster found in research.
*   **H2 [Cluster 1]**:
    *   *Intent*: What/Who?
    *   *Entities*: [List]
*   **H2 [Cluster 2]**:
    *   *Intent*: How/Process?
    *   *Format*: List or Table.

**IV. Semantic Expansion (Authority)**
*   **H2**: Comparison (X vs Y).
*   **H2**: Common Mistakes / Advanced Tips.
*   Context: Demonstrate E-E-A-T.

**V. FAQ (Featured Snippets)**
*   **H2**: FAQ.
*   3-5 "People Also Ask" questions with short (40-60 word) answers.

**VI. Conclusion**
*   Summary + Internal Links + CTA.

#### Constraints
*   **Freshness**: All years/strategies must be **2026** compliant.
*   **Coverage**: Must address **100%** of research intents.

### Phase 3: Output

Generate the outline in Markdown format.

## Self-Check (Read before outputting)

□ Did I include the "Entity Definition" in the intro?
  → Essential for establishing the main entity immediately.

□ Are H2s distinct query clusters?
  → Avoid H2s that just look like generic essay headers; they should map to search demand.

□ Is the "Freshness" year updated to 2026?
  → Check titles and headings.

□ Did I include a specific FAQ section for Featured Snippets?
  → Mandatory for voice search/P0.
