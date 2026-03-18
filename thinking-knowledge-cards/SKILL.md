---
name: thinking-knowledge-cards
description: Turn topics, articles, papers, notes, and source files into linked Obsidian-style knowledge cards or concept nodes in the user's `thinking/` vault style. Use when Codex needs to convert rough material into a concise Chinese knowledge card with 元信息、定义、核心观点、概念关系图、关联概念、延伸、参考、最后更新, while preserving double-bracket links, relation markers, and optional source verification through web search. Also use for requests involving 知识卡片、知识结点、概念卡片、Obsidian卡片、双链整理、thinking 风格整理、知识图谱笔记.
---

# Thinking Knowledge Cards

## Overview

Convert source material into a durable knowledge node rather than a generic study note. Match the existing `thinking/` vault style: concise Chinese writing, viewpoint-driven sections, Obsidian `[[double links]]`, Mermaid concept graphs, and explicit relation markers between concepts.

## Workflow

### 1. Read the artifact first

- Read the target topic, draft, file, article, or pasted notes before writing.
- If the user references a page, paper, or dataset without contents, fetch or open it first.
- Identify whether the target is best written as a concept card, role card, method card, market card, or case-analysis card.

### 2. Distill the core concept

- Write one compact definition that answers what the thing is and why it matters.
- Prefer one knowledge node per file. Do not mix several unrelated concepts into one card.
- Separate the essential concept from examples, anecdotes, and secondary detail.

### 3. Validate important factual claims

- Search the web when the card contains current facts, salary figures, market data, timelines, named reports, or explicit citations.
- Prefer primary or closest-to-primary sources. Read [references/source-validation.md](references/source-validation.md) when choosing links.
- If the claim cannot be verified reliably, either omit it or mark the uncertainty plainly.
- Preserve exact dates when the material uses relative time like “recently” or “today”.

### 4. Shape the card in `thinking/` style

- Default to Chinese.
- Prefer the following section order:
  - `# 标题`
  - `## 元信息`
  - `## 定义`
  - `## 核心观点`
  - `## 概念关系图`
  - `## 关联概念`
  - `## 延伸`
  - `## 参考`
  - `最后更新`
- Add optional middle sections only when the subject clearly needs them:
  - `## 核心技术栈`
  - `## 背景`
  - `## 业务演进脉络`
  - `## 核心概念`
  - `## 详细笔记`

### 5. Build knowledge-network links

- Use Obsidian `[[double links]]` for related notes.
- Use relation markers consistently:
  - `→` for direct prerequisite or foundation
  - `⇒` for downstream implication or application
  - `↔` for comparison or mutual dependence
  - `⋯` for loose but meaningful association
- Keep each relation line explanatory, not just a bare link.
- Add a Mermaid graph when it clarifies the structure of the concept.

### 6. Write viewpoint-driven bullets

- In `核心观点`, lead with a bold short claim, then explain it in one paragraph or a compact list.
- Prefer analytical claims over textbook headings.
- Keep cards dense but not bloated. A good card is scannable in one pass.

## Output Rules

- Match the existing `thinking/` directory voice and structure rather than the generic `learning-notes` template.
- Use tags, difficulty, and update date in the same style as nearby cards.
- Prefer a few high-signal references over a long bibliography.
- When source validation was part of the task, ensure the `参考` section contains the links you actually relied on.
- When writing in Chinese, avoid overusing the “不是……而是……” contrast pattern. Prefer direct statements and straightforward judgment sentences.
- Read [references/thinking-style.md](references/thinking-style.md) when you need the exact card skeleton and style conventions.
