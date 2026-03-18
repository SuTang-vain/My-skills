---
name: tech-blog-writer
description: Write structured technical blog posts and developer-facing articles. Use when Codex needs to draft or revise a technical blog post, tutorial, walkthrough, engineering article, or documentation-style essay with clear sectioning, code examples, best practices, target audience framing, and a concise conclusion. Also use for requests involving 技术博客、教程文章、技术写作、代码示例文章、最佳实践文章、文章润色.
---

# Tech Blog Writer

## Overview

Turn a topic, outline, rough notes, or existing draft into a clear technical article. Keep the writing accurate, well-structured, and readable for the intended audience instead of producing generic marketing copy.

## Workflow

### 1. Frame the article

- Identify the topic, target reader, and the concrete problem the article solves.
- Ask only when the missing constraint is material; otherwise infer a reasonable default audience and state that assumption.
- Decide whether the artifact is a tutorial, conceptual explainer, comparison, incident write-up, or best-practices post.

### 2. Build the article structure

- Start with a specific title.
- Add a short abstract or introduction that explains why the topic matters.
- Organize the body into a clear progression:
  - context or prerequisites
  - core concepts
  - worked examples
  - pitfalls or best practices
  - conclusion and next steps
- Prefer headings that describe the reader outcome, not vague labels.

### 3. Write the technical core

- Explain concepts with concrete examples.
- Include code only when it materially improves understanding.
- Keep snippets correct, readable, and scoped to the point being made.
- Comment complex lines briefly instead of over-explaining trivial code.
- Distinguish clearly between example code, production guidance, and caveats.

### 4. Improve readability

- Use concise language and avoid unnecessary jargon.
- Define specialist terms the first time they appear.
- Use lists, tables, callouts, and short paragraphs when they improve scanability.
- Avoid filler introductions and generic conclusions.

### 5. Close the article

- Summarize the main takeaways.
- Suggest one or two next steps, related topics, or follow-up readings when useful.
- If the article makes factual claims that need verification, attach source links or note that verification is still needed.

## Output Shape

Use this default shape unless the user requests another format:

- Title
- Abstract
- Audience or prerequisites
- Main sections with clear headings
- Code examples with explanation where needed
- Best practices or common mistakes
- Conclusion
- Optional references or further reading

## Working Rules

- Prefer substance over hype.
- Keep code examples runnable or obviously adaptable.
- Match depth to the stated audience.
- If revising a draft, preserve the author's key intent while tightening structure and clarity.
- When writing in Chinese, avoid overusing the “不是……而是……” contrast pattern. Prefer direct statements and straightforward judgment sentences.
- Read [templates/blog-template.md](templates/blog-template.md) when you need a ready-made article skeleton.
- Read [examples/javascript-closure-example.md](examples/javascript-closure-example.md) when you want an example of the expected level of explanation.
