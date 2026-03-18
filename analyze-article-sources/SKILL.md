---
name: analyze-article-sources
description: Analyze blog posts, essays, reports, and academic papers. Use when Codex needs to read an article, blog post, paper, report, PDF, or URL; produce a concise summary; map the section or argument structure; extract important claims, data points, or events; and search the web for source links or primary references that support or contextualize them. Also use for requests involving 摘要、文章结构、论文结构、论点梳理、数据来源、事件来源、出处、参考链接.
---

# Analyze Article Sources

## Overview

Read the target artifact first, then separate interpretation from evidence. Produce a compact summary, reconstruct the article structure in source order, and attach source links for important claims, datasets, and events without inventing citations.

## Workflow

### 1. Acquire the artifact

- Read the article text, URL, PDF, or pasted content before summarizing.
- If the user references a page, paper, or dataset without providing contents, fetch or open it first.
- If the task includes current facts, missing citations, or provenance checks, search the web and gather links before writing the final answer.

### 2. Classify the document

- Identify whether the artifact is a blog post, opinion essay, news analysis, report, whitepaper, or academic paper.
- Capture available metadata: title, author, organization, publication venue, and publication date.
- Note whether the artifact already includes citations, footnotes, figures, or references.

### 3. Build the summary

- State the main thesis or research question first.
- Summarize the supporting logic: method, evidence, examples, or experiments.
- End with the main conclusion, implication, or limitation.
- Keep the summary concise unless the user explicitly asks for depth.

### 4. Map the structure

- List the article's sections in source order.
- Prefer explicit headings when they exist.
- If headings are missing, infer functional sections and label them as inferred.
- For papers, look for: background, question, method, data or experiment, results, discussion, limitations.
- For blog posts or essays, look for: hook or context, core claim, supporting evidence, examples, conclusion or call to action.

### 5. Extract claims that need sourcing

- Pull out claims that are factual enough to justify a link:
  - Numeric statistics
  - Dated events
  - Named studies or papers
  - Statements about organizations, products, regulations, or markets
  - Causal or comparative claims presented as fact
- Separate claims that the article already cites from claims that are asserted without support.
- Preserve exact dates, units, and named entities so the search target stays precise.

### 6. Find and rank sources

- Prefer primary or closest-to-primary sources. Read [references/source-priority.md](references/source-priority.md) when ranking candidate links.
- Use the article's own citations first when they exist and are relevant.
- For papers, prefer DOI pages, publisher pages, arXiv pages, official supplements, and author or lab pages.
- For datasets and statistics, prefer the original dataset, official report, regulator, standards body, or company filing.
- For events, prefer official announcements plus contemporaneous reporting with clear dates.
- If you infer a likely source rather than confirming it directly, label that as an inference.
- If no reliable source can be found, say so explicitly instead of fabricating a citation.

### 7. Produce the output

Use this default shape unless the user requests another format:

#### Summary

- Give a short abstract of the article or paper.

#### Structure

- List the major sections or inferred stages in reading order.
- Add one short line on what each section does.

#### Claims And Sources

Use a compact table when several claims need citation:

| Claim | Source link | Source type | Confidence | Notes |
| --- | --- | --- | --- | --- |

- Keep one row per distinct claim or tightly related claim cluster.
- Reuse one source for multiple rows only when the source clearly covers each row.
- Mark `High`, `Medium`, or `Low` confidence based on how directly the source supports the claim.

#### Gaps Or Caveats

- List unsupported claims, ambiguous terminology, missing dates, or places where the article overstates the evidence.

## Working Rules

- Distinguish clearly between the article's own argument and externally verified facts.
- Prefer paraphrase over long quotation; quote only when wording matters.
- Preserve uncertainty. If a paper has weak evidence, a blog post cites stale data, or an event link is secondary rather than primary, say that plainly.
- When the user asks only for summary and structure, keep sourcing focused on the most material claims instead of exhaustively linking every sentence.
- When writing in Chinese, avoid overusing the “不是……而是……” contrast pattern. Prefer direct statements and straightforward judgment sentences.
