---
name: learning-notes
description: Create structured learning notes from a topic, article, lecture, draft, or source file. Use when Codex needs to explain concepts, define terms, connect related ideas, organize study material, generate review-friendly notes, or convert rough content into a reusable knowledge document. Also use for requests involving 学习笔记、知识梳理、概念解释、术语说明、知识关联、复习提纲、课程笔记.
---

# Learning Notes

## Overview

Convert raw study material into notes that are easy to learn from and easy to revisit later. Focus on concept clarity, relationships between ideas, and a layout that supports review instead of dumping unstructured summaries.

## Workflow

### 1. Read and classify the material

- Accept a topic, pasted text, article, file, or rough notes.
- Determine whether the material is conceptual, procedural, comparative, or problem-solving oriented.
- Identify the expected learner level if the user provides it; otherwise infer a reasonable default.

### 2. Extract the knowledge units

- Identify key concepts, terms, definitions, methods, and examples.
- Separate core ideas from supporting details.
- Pull out prerequisites, common confusions, and important distinctions.

### 3. Explain and connect

- Define each important concept in plain language first.
- Add examples, short analogies, or code snippets when they reduce ambiguity.
- Show relationships such as prerequisite, contrast, hierarchy, and application.
- Call out what is easy to confuse or easy to forget.

### 4. Organize for review

- Use a stable note structure with clear headings.
- Include quick review sections such as takeaways, flash review bullets, or common pitfalls.
- If visual structure helps, use tables or Mermaid diagrams.
- Keep the note compact enough to scan later.

### 5. Add references when useful

- Link to primary learning resources, official docs, or the source artifact when that helps later review.
- If the note depends on current facts or external references, verify them before presenting them as fact.

## Output Shape

Use this default shape unless the user requests another format:

- Topic
- Metadata or scope
- Learning goals
- Core concepts
- Concept relationships
- Detailed notes or worked examples
- Common pitfalls
- Quick review
- References or follow-up resources

## Working Rules

- Optimize for future recall, not just first-pass explanation.
- Prefer precise definitions over motivational filler.
- Use examples sparingly but concretely.
- Preserve uncertainty when a concept is still ambiguous in the source material.
- When writing in Chinese, avoid overusing the “不是……而是……” contrast pattern. Prefer direct statements and straightforward judgment sentences.
- Read [templates/note-template.md](templates/note-template.md) when you need a ready-made note structure.
- Read [examples/react-hooks-example.md](examples/react-hooks-example.md) when you want a model for note depth and explanatory style.
